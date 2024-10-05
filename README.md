# Dynamic Retail Data Analysis

## Project Overview
**Dynamic Retail Data Analysis** is a comprehensive project focused on analyzing sales data from various retail stores to uncover valuable insights and trends that can enhance business decision-making. The analysis emphasizes the influence of key factors, including holidays, promotional markdowns, temperature variations, and fuel prices on weekly sales performance.

## Dataset
The project utilizes the [Retail Dataset](https://www.kaggle.com/datasets/manjeetsingh/retaildataset) by Manjeet Singh, which encompasses a variety of features, including:

- Store details
- Weekly sales figures
- Economic indicators (CPI, unemployment rates)
- Promotional markdowns (Markdown1-5)

## Steps Involved

### 1. Import Necessary Libraries
The following Python libraries are used for data manipulation and visualization:
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations and data handling.
- **Matplotlib**: For data visualization.
- **Seaborn**: For enhanced data visualizations.

### 2. Load and Inspect the Data
The project begins by loading the **Features**, **Sales**, and **Stores** datasets, followed by inspecting the first few rows to grasp their structure.

### 3. Data Cleaning
To ensure data quality, the datasets are thoroughly checked for missing values. Key cleaning steps include:
- Filling missing markdown values with **0**.
- Forward-filling missing economic indicators such as CPI and unemployment rates.
- Converting date columns into the datetime format.

### 4. Merge the Datasets
The **Sales**, **Features**, and **Stores** datasets are merged on common columns (`Store`, `Date`, `IsHoliday`) to create a unified dataset for comprehensive analysis.

### 5. Exploratory Data Analysis (EDA)
The EDA phase involves several key analyses:
- **Total Sales Over Time**: Analyzing weekly sales trends over time using line plots.
- **Holiday vs. Non-Holiday Sales**: Comparing average sales during holidays versus non-holidays with bar plots.
- **Impact of Markdowns**: Investigating the effect of promotional markdowns on sales performance.
- **Impact of External Factors**: Analyzing how temperature and fuel prices affect sales.

### 6. Conclusions/Findings
The project concludes with several key findings, including:
- A **7.13%** increase in sales during holidays.
- A **1.92%** rise in sales during weeks with promotional markdowns.
- The highest sales occur during moderate temperature conditions.
- Low fuel prices correlate with increased sales.

## Recommendations for Future Sales Strategies

1. **Holiday Sales**: Plan and prepare for holiday sales in advance, focusing on popular products.
2. **Markdown Impacts**: Implement strategic markdowns during promotional weeks to boost sales, like offering discounts on high-demand products.
3. **Temperature Effect**: Optimize product placement and marketing strategies to target customers during "Moderate" temperature conditions.
4. **Fuel Prices**: Monitor fuel prices and adjust pricing strategies accordingly to maximize sales during low fuel.
