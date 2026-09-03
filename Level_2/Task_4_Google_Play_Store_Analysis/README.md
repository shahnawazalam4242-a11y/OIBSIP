# Unveiling the Android App Market

## Google Play Store Data Analysis

### Project Overview

This project performs a comprehensive analysis of the Google Play Store ecosystem using Python and Jupyter Notebook.

The analysis focuses on data cleaning, application categories, ratings, installations, pricing trends and user sentiment. The project uses separate Google Play Store applications and user reviews datasets.

---

## Objectives

The main objectives of this project are to:

- Clean and prepare real-world Google Play Store data.
- Analyse the distribution of applications across categories.
- Identify the most saturated application categories.
- Examine application ratings and user satisfaction.
- Investigate the relationship between application size and installations.
- Compare free and paid applications.
- Analyse the price distribution of paid applications.
- Estimate theoretical gross revenue by category.
- Perform sentiment analysis on user reviews.
- Analyse positive and negative sentiment across app categories.
- Provide data-driven recommendations for new app developers.

---

## Technologies Used

- Python
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- seaborn
- TextBlob
- Plotly

---

## Datasets

This project uses two datasets:

### 1. Google Play Store Apps Dataset

The dataset contains information about Android applications, including:

- App name
- Category
- Rating
- Number of reviews
- Application size
- Number of installs
- Application type
- Price
- Content rating
- Genres
- Last updated date

### 2. Google Play Store User Reviews Dataset

This dataset contains user reviews associated with Google Play Store applications.

The review text is analysed to classify user sentiment as:

- Positive
- Neutral
- Negative

---

## Data Cleaning

The following data cleaning processes were performed:

- Converted `Installs` from text values such as `10,000+` into numerical values.
- Converted `Reviews` into a numerical data type.
- Removed currency symbols and converted `Price` into numerical format.
- Standardised application sizes into megabytes using a new `Size_MB` variable.
- Converted `Last Updated` into datetime format.
- Removed duplicate rows.
- Removed duplicate application records.
- Handled missing values based on their importance to the analysis.
- Cleaned and prepared the user reviews dataset for sentiment analysis.

---

## Exploratory Data Analysis

### Category Analysis

The distribution of applications across Google Play Store categories was analysed to identify the most saturated and competitive categories.

### Ratings Analysis

The project examines:

- The overall distribution of application ratings.
- Average application ratings by category.

### Application Size and Installs

A scatter plot and Pearson correlation analysis were used to investigate the relationship between application size and installation numbers.

### Pricing Analysis

The pricing analysis includes:

- Free versus paid application distribution.
- Price distribution of paid applications.
- Theoretical gross revenue by application category.

The revenue calculation is an estimate based on application price and installation numbers and does not represent actual revenue.

---

## Sentiment Analysis

User reviews were analysed using the TextBlob library.

Each review was classified as:

- Positive
- Neutral
- Negative

The project also merges user reviews with application category information to analyse sentiment patterns across different categories.

---

## Interactive Visualisation

An interactive Plotly visualisation compares application categories based on:

- Number of applications
- Average rating
- Total installations

This provides an interactive view of market competition, user satisfaction and application reach.

---

## Key Insights

The analysis provides several useful insights for developers planning to launch a new application:

1. **Market Competition:** Highly saturated categories may involve stronger competition, making product differentiation important.

2. **User Feedback:** Ratings and negative reviews can reveal customer problems and opportunities for application improvement.

3. **Monetisation:** The dominance of free applications demonstrates the importance of selecting an appropriate monetisation strategy, such as advertising, subscriptions or in-app purchases.

---

## How to Run the Project

### Step 1: Install Required Libraries

Run the following command in Jupyter Notebook:

```python
%pip install pandas numpy matplotlib seaborn textblob plotly
```

### Step 2: Download the Datasets

Make sure the following dataset files are available in your project folder:

```text
googleplaystore.csv
googleplaystore_user_reviews.csv
```

### Step 3: Open the Jupyter Notebook

Open the project notebook:

```text
level2_Task_4_Google_Play_Store_Analysis.ipynb
```

### Step 4: Run the Notebook

Run all cells sequentially from the beginning.

In JupyterLab, you can use:

```text
Run → Run All Cells
```

### Step 5: View the Results

The notebook will generate:

- Data cleaning results
- Category analysis visualisations
- Ratings analysis
- Size versus installs analysis
- Pricing analysis
- Sentiment analysis
- Sentiment by category analysis
- Interactive Plotly visualisation
- Final business insights