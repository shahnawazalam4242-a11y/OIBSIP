# Predicting House Prices with Linear Regression

## Level 2 – Task 1 | Machine Learning Project

---

## Project Overview

This project develops and evaluates a Linear Regression machine learning model to predict house prices using housing characteristics, geographical information, property age, population-related variables, income and location categories.

The project follows an end-to-end machine learning workflow, beginning with Exploratory Data Analysis (EDA) and data preprocessing and continuing through model training, evaluation and interpretation.

The target variable used for prediction is:

`median_house_value`

---

## Project Objectives

The main objectives of this project are to:

- Perform Exploratory Data Analysis (EDA) on the housing dataset.
- Identify missing values, duplicate records and data types.
- Analyse the distribution of house prices.
- Select relevant features for predicting house prices.
- Handle missing values using an appropriate preprocessing strategy.
- Encode categorical variables using One-Hot Encoding.
- Analyse correlations between numerical features and house prices.
- Split the dataset into training and testing datasets using an 80/20 split.
- Train a Linear Regression model using Scikit-learn.
- Evaluate model performance using MSE, RMSE and R² score.
- Compare actual and predicted house prices.
- Analyse prediction residuals.
- Interpret model coefficients to identify influential features.
- Compare Linear Regression with Ridge Regression.

---

## Dataset

This project uses the California Housing dataset.

The dataset contains information about housing characteristics and geographical areas in California.

### Dataset Features

| Feature | Description |
|---|---|
| `longitude` | Geographical longitude of the housing area |
| `latitude` | Geographical latitude of the housing area |
| `housing_median_age` | Median age of houses |
| `total_rooms` | Total number of rooms |
| `total_bedrooms` | Total number of bedrooms |
| `population` | Population within the housing area |
| `households` | Number of households |
| `median_income` | Median income of households |
| `ocean_proximity` | Location category based on proximity to the ocean |
| `median_house_value` | Median house value (target variable) |

### Target Variable

`median_house_value`

The dataset does not contain a direct property-area measurement. Therefore, `total_rooms` and `total_bedrooms` are used as proxy indicators of property size.

---

## Technologies Used

This project was developed using:

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Structure

```text
House_Price_Prediction/
│
├── housing.csv
├── Level_2_Task_1_House_Price_Prediction.ipynb
└── README.md
```

---

## Project Workflow

### 1. Data Loading and Initial Inspection

The dataset was loaded using pandas and inspected to understand:

- Dataset dimensions
- Column names
- Data types
- Missing values
- Duplicate records

### 2. Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the characteristics and distribution of the dataset.

The analysis includes:

- Descriptive statistics
- Missing value analysis
- Duplicate record analysis
- Distribution of the target variable
- Correlation analysis

### 3. Feature Selection

Relevant features were selected based on their potential relationship with house prices.

#### Location Features

- `longitude`
- `latitude`
- `ocean_proximity`

#### Housing Characteristics

- `housing_median_age`
- `total_rooms`
- `total_bedrooms`
- `households`

#### Area Characteristics

- `population`

#### Economic Feature

- `median_income`

### 4. Data Preprocessing

The dataset was prepared for machine learning using a Scikit-learn preprocessing pipeline.

#### Missing Value Handling

Numerical missing values were handled using median imputation.

Categorical missing values were handled using most frequent value imputation.

#### Categorical Data Encoding

The `ocean_proximity` feature was converted into numerical features using One-Hot Encoding.

#### Feature Scaling

Numerical variables were standardised using `StandardScaler`.

A preprocessing pipeline was used to reduce the risk of data leakage and ensure that preprocessing was applied consistently.

### 5. Correlation Analysis

A correlation heatmap was created to analyse relationships between numerical variables and `median_house_value`.

### 6. Train-Test Split

The dataset was divided into:

- 80% training data
- 20% testing data

The training data was used to develop the model, while the testing data was used to evaluate its performance on unseen observations.

---

## Machine Learning Models

### Linear Regression

A Linear Regression model was trained to predict median house values based on the selected features.

Linear Regression provides an interpretable baseline model and allows the relationship between predictor variables and house prices to be analysed through model coefficients.

### Ridge Regression

A Ridge Regression model was also developed as a regularised alternative to Linear Regression.

The purpose of this comparison was to evaluate whether regularisation could improve model performance.

---

## Model Evaluation

The models were evaluated using the following metrics:

### Mean Squared Error (MSE)

Measures the average squared difference between actual and predicted house prices.

### Root Mean Squared Error (RMSE)

Measures the typical prediction error in the same unit as the target variable.

### R² Score

Measures the proportion of variation in house prices explained by the model.

---

## Visualisations

The project includes the following visualisations:

- Distribution of median house values
- Correlation heatmap
- Feature correlation analysis
- Actual versus predicted house prices
- Residual plot
- Residual distribution
- Coefficient analysis
- Most influential features

---

## Model Interpretation

Coefficient analysis was performed to understand the influence of individual features on predicted house prices.

- A positive coefficient indicates a positive relationship with predicted house value.
- A negative coefficient indicates an inverse relationship with predicted house value.
- Features with larger absolute coefficient values have a stronger influence on the model after preprocessing.

The coefficients represent relationships identified by the model and should not automatically be interpreted as causal relationships.

---

## Key Findings

- House prices are influenced by a combination of geographical, housing and economic factors.
- Location-related features provide valuable information for predicting house values.
- Housing characteristics such as rooms and property age contribute to house price predictions.
- Median income is an important economic indicator for housing value prediction.
- Actual versus predicted price analysis helps visually assess model performance.
- Residual analysis provides insights into potential patterns in prediction errors.
- Comparing Linear Regression and Ridge Regression provides additional insights into model performance.

---

## How to Run the Project

### Step 1: Download or Clone the Project

Ensure the following files are available in the same project folder:

```text
housing.csv
Level_2_Task_1_House_Price_Prediction.ipynb
README.md
```

### Step 2: Install Required Libraries

Run:

```python
%pip install pandas numpy matplotlib seaborn scikit-learn
```

### Step 3: Open the Jupyter Notebook

Open:

```text
Level_2_Task_1_House_Price_Prediction.ipynb
```

### Step 4: Run the Notebook

Run all cells sequentially from the beginning.

Use:

```text
Run → Run All Cells
```

### Step 5: View the Results

The notebook will generate:

- Exploratory Data Analysis results
- Data quality checks
- Target variable distribution
- Correlation analysis
- Data preprocessing
- Linear Regression predictions
- Model evaluation metrics
- Actual versus predicted visualisation
- Residual analysis
- Coefficient analysis
- Ridge Regression comparison
- Final conclusions

---

## Future Improvements

Potential improvements include:

- Feature engineering using ratios and housing-density variables.
- Log transformation of highly skewed variables.
- Hyperparameter tuning for Ridge Regression.
- Comparison with Lasso Regression.
- Testing advanced machine learning algorithms.
- Performing cross-validation for more robust model evaluation.

---

