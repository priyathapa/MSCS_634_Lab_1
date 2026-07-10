# MSCS 634 – Lab 1: Data Visualization, Preprocessing, and Statistical Analysis

## Overview

This lab demonstrates the application of data visualization, data preprocessing, and statistical analysis techniques using Python in a Jupyter Notebook environment. The objective is to explore a real-world dataset, prepare it for analysis, and gain meaningful insights through descriptive statistics and visualizations.

---

## Dataset

This lab uses the **USA House Prices Dataset** obtained from Kaggle.

**Dataset Source:**  
https://www.kaggle.com/datasets/fratzcan/usa-house-prices

The dataset contains residential property information, including:

- House price
- Number of bedrooms and bathrooms
- Living area and lot size
- Number of floors
- Waterfront status
- Property condition
- Year built and renovation year
- City and location information

The combination of numerical and categorical variables makes this dataset well suited for data visualization, preprocessing, and statistical analysis.

---

## Project Objectives

The following tasks were completed as part of this lab:

- Loaded the dataset into a Pandas DataFrame.
- Explored the dataset using descriptive statistics.
- Created multiple visualizations to examine relationships and distributions within the data.
- Performed data preprocessing by:
  - Checking for missing values
  - Detecting and removing outliers using the IQR method
  - Applying data reduction through sampling and column elimination
  - Performing Min-Max Scaling
  - Discretizing house prices into categorical groups
- Conducted statistical analysis, including:
  - General dataset overview
  - Measures of central tendency
  - Measures of dispersion
  - Correlation analysis

---

## Key Insights

Several meaningful insights were obtained during the analysis:

- Larger homes generally have higher selling prices, indicating a positive relationship between living area and house price.
- House prices exhibit a right-skewed distribution due to the presence of high-value properties.
- Outlier detection using the IQR method identified several unusually expensive houses, which were removed before further analysis.
- Min-Max Scaling successfully normalized selected numerical variables to a common range.
- Discretizing house prices into Low, Medium, and High categories simplified the interpretation of price ranges.
- Correlation analysis revealed that variables such as living area and bathrooms are positively associated with house prices.

---

## Repository Structure

```
MSCS634_Lab1/
│
├── MSCS634_Lab1.ipynb
├── USA Housing Dataset.csv
├── README.md
└── screenshots/
    ├── Data Collection/
    ├── Data Visualization/
    ├── Data Preprocessing/
    └── Statistical Analysis/
```

---

## Challenges and Decisions

The dataset contained no missing values, so no imputation or removal of incomplete records was necessary. During preprocessing, the IQR method was selected for outlier detection because it effectively identifies extreme values without making assumptions about the underlying distribution. Random sampling and feature elimination were applied to demonstrate data reduction techniques, while Min-Max Scaling and discretization were used to prepare the data for future machine learning applications.

---

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
