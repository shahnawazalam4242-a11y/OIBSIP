# Exploratory Data Analysis on Retail Sales Data

## Level 1 – Task 1 | Data Analytics Project

## Project Overview

This project performs Exploratory Data Analysis (EDA) on a retail sales dataset to identify sales trends, customer behaviour and product category performance.

The analysis uses Python to explore the dataset, create visualisations and generate actionable business insights.

## Technologies Used

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- Seaborn

## Dataset

The dataset contains retail transaction information with the following features:

| Feature | Description |
|---|---|
| Transaction ID | Unique transaction identifier |
| Date | Transaction date |
| Customer ID | Unique customer identifier |
| Gender | Customer gender |
| Age | Customer age |
| Product Category | Purchased product category |
| Quantity | Number of items purchased |
| Price per Unit | Price of one item |
| Total Amount | Total transaction value |

Note: The dataset contains product categories rather than individual product names. Therefore, product analysis focuses on category-level performance.

## Analysis Performed

The project includes:

- Dataset inspection and data quality checks
- Missing value and duplicate analysis
- Descriptive statistics
- Monthly sales trend analysis
- Quarterly sales trend analysis
- Customer age and gender analysis
- Product category performance analysis
- Revenue analysis by product category
- Correlation heatmap
- Additional customer spending analysis
- Business recommendations

## Key Visualisations

- Monthly sales trends
- Quarterly sales trends
- Customer age distribution
- Gender breakdown
- Product category sales performance
- Revenue by product category
- Correlation heatmap
- Customer spending insights

## Key Findings

The analysis shows that:

- Sales performance varies across different time periods.
- Customer purchasing behaviour differs across demographic groups.
- Product categories vary in terms of sales quantity and revenue.
- High sales volume does not always result in the highest revenue.
- Customer age groups may show differences in average spending behaviour.

## Business Recommendations

1. Maintain appropriate inventory for high-demand product categories.
2. Focus marketing efforts on high-revenue products and customer segments.
3. Use customer demographic data to develop targeted promotions.
4. Further investigate seasonal sales patterns to improve sales planning.

## How to Run the Project

### Step 1: Install Required Libraries

```python
%pip install pandas numpy matplotlib seaborn
```

### Step 2: Open the Notebook

Open:

```text
Level_1_Task_1_Retail_Sales_EDA.ipynb
```

### Step 3: Run the Project

Run all notebook cells sequentially using:

```text
Run → Run All Cells
```

## Project Structure

```text
Retail_Sales_EDA/
│
├── retail_sales_dataset.csv
├── Level_1_Task_1_Retail_Sales_EDA.ipynb
└── README.md
```
