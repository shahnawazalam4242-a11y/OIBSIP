# Employee Data Cleaning

## Level 1 – Task 3 | Data Analytics Project

## Project Overview

This project demonstrates a complete data cleaning process using a messy employee dataset. The objective was to identify data quality issues and transform the original data into a clean, analysis-ready dataset using Python, pandas and NumPy.

## Dataset

The original employee dataset contains information such as:

- Employee ID
- Name
- Age
- Department and Region
- Employment Status
- Join Date
- Salary
- Email
- Phone Number
- Performance Score
- Remote Work Status

The cleaning process also separates `Department_Region` into individual `Department` and `Region` columns.

## Technologies Used

- Python
- Jupyter Notebook
- pandas
- NumPy

## Data Cleaning Process

The project includes:

1. **Data Quality Assessment**  
   Checked missing values, duplicate records, data types and value anomalies.

2. **Missing Value Handling**  
   Missing values in numerical columns such as Age and Salary were handled using appropriate imputation methods.

3. **Duplicate Analysis**  
   Checked for duplicate rows and duplicate employee IDs.

4. **Data Standardisation**  
   Standardised inconsistent text values, names, employment information and other categorical data.

5. **Data Type Correction**  
   Converted columns into appropriate formats, including dates, numerical values and IDs.

6. **Outlier Detection**  
   Used the IQR method to identify potential outliers in numerical columns.

7. **Before vs After Comparison**  
   Compared data quality before and after the cleaning process.

8. **Cleaned Dataset Export**  
   Saved the final analysis-ready dataset as a new CSV file.

## Project Structure

```text
Employee_Data_Cleaning/
│
├── Messy_Employee_Dataset.csv
├── Task_3_Data_Cleaning.ipynb
├── Cleaned_Employee_Dataset.csv
└── README.md
```

## How to Run

### Step 1: Install Required Libraries

```python
%pip install pandas numpy
```

### Step 2: Open the Notebook

```text
Task_3_Data_Cleaning.ipynb
```

### Step 3: Run All Cells

Run the notebook from beginning to end:

```text
Run → Run All Cells
```

The cleaned dataset will be saved as:

```text
Cleaned_Employee_Dataset.csv
```

## Key Learning Outcomes

- Data quality assessment
- Missing data handling
- Duplicate removal
- Data standardisation
- Data type correction
- Outlier detection
- Data validation

