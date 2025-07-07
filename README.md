# Walmart Sales Analysis and Marketing Recommendations

This project analyzes Walmart sales data to uncover trends, generate insights, and provide actionable marketing recommendations.

## Setup Instructions

1. **Clone the repository**
2. **Create a virtual environment**
   ```bash
   python -m venv walmart-virt
   ```
3. **Activate the virtual environment**
   - On Windows:
     ```bash
     walmart-virt\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source walmart-virt/bin/activate
     ```
4. **Install required packages**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn jupyter openpyxl
   ```
5. **Start Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

## Usage
- Open your browser to the Jupyter Notebook interface.
- Create or open notebooks to begin your analysis.

## Project Goals
- Analyze sales trends and seasonality
- Identify key drivers of sales
- Provide actionable marketing recommendations

---
## 1️⃣ Business Understanding
Goal: Analyze Walmart’s weekly sales to identify factors influencing sales and recommend strategies to increase sales.

Objectives:

Evaluate the impact of holidays, temperature, fuel price, CPI, and unemployment on sales.

Compare store-specific performance to identify high and low performers.

Identify seasonality and trends in sales.

Provide actionable marketing and operational recommendations.

## 2️⃣ Data Understanding
Your dataset (Walmart_sales_analysis.csv) contains:

- Store: Store number

- Date: Week start date

- Weekly_Sales: Sales for the week

- Holiday_Flag: 1 if the week includes a major holiday, else 0

- Temperature: Average temperature for the week

- Fuel_Price: Fuel price in the region

- CPI: Consumer Price Index

- Unemployment: Unemployment rate


✅ Check missing values and data types
✅ Summarize data statistics
✅ Visualize distributions and correlations


## 3️⃣ Data Preparation
Convert Date to datetime format.

Create Year, Month, Week features.

Check for and handle missing values if present.

Check outliers using IQR or Z-scores for Weekly_Sales, Temperature, Fuel_Price, CPI, Unemployment.

Normalize/scale variables if needed for modeling.

## 4️⃣ Modeling
We will not build predictive ML models for now, but:
✅ Perform hypothesis testing
✅ Use statistical tests to check relationships and significance

* Hypothesis Testing
Holiday Impact:

Null (H0): Holidays do not significantly impact weekly sales.

Alternate (H1): Holidays significantly increase weekly sales.

Using two-sample t-test between holiday and non-holiday weeks.


## 5️⃣ Evaluation
Insights will be evaluated for business relevance:

10 Analytical Questions

1️⃣ What is the total and average weekly sales across all stores?

2️⃣ Which stores have the highest and lowest total sales?

3️⃣ How do sales vary across months and seasons?

4️⃣ Which factors significantly impact weekly sales?

5️⃣ What is the correlation between temperature and weekly sales?

6️⃣ What is the correlation between fuel price and weekly sales?

7️⃣ What is the correlation between CPI and weekly sales?

8️⃣ What is the correlation between unemployment and weekly sales?

9️⃣ Are there any clear trends in sales over time?

🔟 What are actionable recommendations based on the above insights for increasing sales?


## 6️⃣ Deployment
Present insights and recommendations in:

Clean visualizations (line plots, boxplots, heatmaps)

Summary tables

Actionable recommendations aligned with your provided PDF strategy document
