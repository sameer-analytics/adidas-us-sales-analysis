# Adidas US Sales Analysis

---

## Project Description

This project analyzes the **Adidas US Sales dataset** to uncover actionable insights, optimize business strategies, and enhance decision-making processes.  
The analysis focuses on key areas such as regional and product performance, sales trends, and channel effectiveness, providing valuable insights for strategic planning and revenue optimization.

---

## Dataset

**Source:** Kaggle  

- **Key Columns:**  
  - **Retailer**: Name of the retailer associated with the sales.  
  - **Invoice Date**: Date of the invoice for the sales transaction.  
  - **Region**: Geographic area of the sales.  
  - **State**: State where the sales occurred.  
  - **City**: City where the sales occurred.  
  - **Product**: Type of product sold.  
  - **Price per Unit**: Selling price per unit of the product.  
  - **Units Sold**: Number of units sold.  
  - **Revenue**: Total sales revenue generated.  
  - **Profit**: Net profit earned from the sales.  
  - **Sales Method**: Channel of sale (e.g., online, outlet, in-store).  
  - **Profit Margin**: Ratio of profit to revenue, expressed as a percentage.  
  - **Profit per Unit Sold**: Profit earned per unit of the product sold.  

- **Size:** 9,638 rows and 13 columns.

---

## Steps Performed

### 1. Import Libraries
We import the necessary libraries that will allow us to manipulate, analyze, and visualize the data effectively.
- **Libraries Used**:
  - **numpy**: For numerical computation (used when performing calculations on data).
  - **pandas**: For data manipulation, cleaning, and analysis, especially for handling CSV files.
  - **matplotlib.pyplot**: For creating visualizations (graphs, charts) to better understand the data.
These libraries form the foundation for the data analysis and visualization steps in this project.

### 2. Load the Data
- To load the data set i have used directory path. I have uploaded the uncleaned data set inside the data sub folder and use this directory "../01_Data/01_Adidas US Sales uncleaned data set.csv" ton convert the data set into a data frame using pr.read_csv() code and inside the parethesis i have used the directory(given).

**Libraries Used**:
  - **pandas**: For data manipulation and analysis, especially useful for reading CSV files into DataFrames.

**Action**: The dataset is loaded into a pandas DataFrame using the **read_csv()** method. This allows us to easily manipulate, clean, and analyze the data in a structured format.

**Verification**: Display the first few rows using **df.head()** to confirm that the dataset has been loaded properly. This helps us ensure the data is correctly read and ready for the next steps in the analysis process.


### 3. Data Exploration
- Loaded the dataset into a pandas DataFrame.
- Displayed the first 10 rows to get an initial view of the data.
- Retrieved the column names to understand the dataset's structure.
- Checked the DataFrame's information to analyze data types and non-null counts of columns.
- Generated summary statistics to gain insights into the numerical data.
- Checked for missing values to ensure data completeness.
- Identified duplicate rows in the dataset.
- Examined duplicate columns by transposing the dataset for easier detection.
- Checked unique values in the **region**, **product**, and **sales_method** columns to understand the distribution of categorical data.


### 2. Data Cleaning
- Removed unnecessary columns: **sales_id**, **retailer_id**.
- Renamed columns for better understanding: **total_sales** to **revenue**, **operating_profit** to **profit**.
- Added a new column: **profit_margin** to represent profit as a percentage of revenue.
- Changed the data type of categorical columns to **string** for consistency and memory optimization.
- Converted the **invoice_date** column to **datetime** format to ensure proper date handling.


### 3. Exploratory Data Analysis (EDA)
- Examined distributions and relationships between variables.
- Analyzed trends over time.
- Investigated correlations between numerical columns.
- Explored statistical values such as min, max, mean, etc., for numerical columns like revenue, profit, profit_margin, price_per_unit, and units_sold.
- Detected outliers using the standard deviation method and visualized distributions through histograms.
- Identified the most and least sold products and examined month-wise sales, profit, and product trends.
- Generated a correlation matrix to explore relationships between numerical variables.

### 4. Data Visualization
- **Revenue and Profit by Region:**  
  Visualized profit and revenue for each region using bar charts to compare the performance of different regions.
- **Revenue and Profit by Product:**  
  Plotted bar charts to show how revenue and profit vary by product.
- **Monthly Sales Analysis:**  
  Analyzed product sales trends over the months by plotting a line chart for product units sold across each month.
- **Sales by Channel:**  
  Analyzed the performance of different sales channels (e.g., Online, Outlet, In-store) using a bar chart to show product sales by channel.
- **State-Level Profit Analysis:**  
  Displayed a bar chart for state-wise profit analysis and another for units sold across different states.
- **Units Sold vs. Profit Margin:**  
  Plotted a scatter plot to examine the correlation between the number of units sold and the profit margin, highlighting the relationship between these two variables.

---

## Key Insights

### Insight 1: Profit and Revenue by Region
- The West Region leads in both profit and revenue, while the Midwest lags behind. Focus on maintaining growth in the West and improving marketing strategies in the Midwest.

### Insight 2: Revenue and Profit by Product
- Men's Street Footwear drives the highest sales and profit, while Women's Athletic Footwear underperforms. Improve quality and design for the latter while expanding distribution of the former.

### Insight 3: Monthly Sales Trend
- August sees the highest sales, and June the lowest. Leverage August’s success by applying similar strategies to June and plan for consistent sales growth post-August.

### Insight 4: Sales by Method
- Online sales dominate, followed by outlet sales, while in-store sales are the lowest. Enhance online sales strategies and improve in-store experiences with discounts and promotions.

### Insight 5: Profit and Sales by State
- California, Texas, and New York are top performers, while states like Nebraska, Maryland, and Minnesota underperform. Focus on maintaining strength in high-performing states and explore growth opportunities in underperforming areas.

### Insight 6: Units Sold and Profit Margin
- Low unit sales correlate with low profit margins, but high sales can result in higher profits. Optimize costs in low-performing regions and focus on profitable products and regions.

---

## Recommendations

### Profit and Revenue Analysis by Region
- **Recommendations:** Maintain the growth trajectory in the West region by continuing effective marketing and distribution strategies.  
  Implement new marketing strategies, offer sales discounts, and assess underlying issues to improve profitability in the Midwest region.

### Revenue and Profit Analysis by Product
- **Recommendations:** Continue focusing on selling and increasing the distribution of Men's Street Footwear. Improve the quality and design of Women's Athletic Footwear, and gather user feedback to enhance product appeal.

### Monthly Product Sales Trend
- **Recommendations:** Identify and replicate factors driving high sales in August to apply them to lower-performing months.  
  Offer targeted promotions or discounts in June to attract more customers and increase sales, and develop strategies to maintain sales momentum post-August.

### Sales by Method Analysis
- **Recommendations:** Continue to enhance online sales by improving customer experience, marketing strategies, and delivery systems.  
  Strengthen the presence of outlet stores in high-demand areas to boost their sales and focus on improving in-store sales by offering special discounts, events, and promotions.

### Profit and Sales Analysis by State
- **Recommendations:** Maintain strong performance in high-performing states like California, Texas, and New York by continuing targeted marketing and local promotions.  
  Investigate underperformance in states like Nebraska, Maryland, and Minnesota, and consider offering localized promotions or improving product distribution.

### Units Sold and Profit Margin Analysis
- **Recommendations:** For regions with low unit sales and low profit margins, focus on optimizing cost structures and revising pricing strategies.  
  Identify and capitalize on regions or products with higher profit margins and replicate these strategies to ensure consistent profitability.

---

## Technologies Used

- **Programming Language:** Python  
- **Libraries:** pandas, numpy, matplotlib ,seaborn 
- **Development Environment:** jupyter notebook 
- **Dataset Format:** CSV  

---

# Folder Structure

- **01_Data** Contains the raw dataset and cleaned dataset used in the project.
- **02_scripts:** Includes Python scripts for different stages of the analysis:
  - **a_Common_imports.ipynb:** Script for importing necessary libraries.
  - **b_Data_load.ipynb:** Script for loading the dataset.
  - **c_Data_exploration.ipynb:** Script for initial exploration of the dataset.
  - **d_Data_Cleaning.ipynb:** Script for data cleaning processes.
  - **e_EDA.ipynb:** Script for exploratory data analysis.
  - **f_data_visualization(code).ipynb:** Script for creating visualizations.
- **03_output:** Stores outputs generated during the project:
  - **01_visualizations(images):** Contains visualizations such as bar charts, line charts, and scatter plots.
  - **02_reports:** Includes markdown reports summarizing key findings and insights.
- **README.md:** Documentation describing the project overview, steps, and insights.
- **requirements.txt:** Lists all the Python libraries required to run the project.
