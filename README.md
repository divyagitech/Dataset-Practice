# EDA and Linear Regression with Python

This repository provides a Jupyter Notebook demonstrating Exploratory Data Analysis (EDA) and Linear Regression modeling on an Ecommerce dataset. The analysis guides you through understanding the data, visualizing relationships, and building a regression model to predict customer spending.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Requirements](#requirements)
- [Usage](#usage)
- [Key Steps in the Notebook](#key-steps-in-the-notebook)
- [Results](#results)
- [License](#license)

## Overview

The notebook `EDA_Linear_Regression.ipynb` walks through:

- Loading and inspecting the dataset using pandas
- Performing EDA with summary statistics and visualization (using matplotlib and seaborn)
- Feature selection for regression
- Model building with scikit-learn's LinearRegression
- Evaluation and visualization of regression results

## Dataset

The dataset used in the notebook is named "Ecommerce Customers" and contains the following columns:

- **Email**: Customer email address
- **Address**: Customer address
- **Avatar**: Customer avatar color
- **Avg. Session Length**: Average session time on the website
- **Time on App**: Average time spent on the app
- **Time on Website**: Average time spent on the website
- **Length of Membership**: Number of years as a customer
- **Yearly Amount Spent**: Target variable — yearly customer spending

> **Note:** You will need to provide the dataset file (e.g., `Ecommerce Customers.csv`) and update the file path as needed in the notebook.

## Features

- Pandas-based data exploration and summary
- Visualizations: scatter plots, histograms, pair plots, and joint plots (seaborn)
- Correlation and feature relationship analysis
- Model training and testing split
- Building a multiple linear regression model
- Interpreting coefficients and feature impact
- Model evaluation 

## Requirements

- Python 3.11
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Install dependencies via pip if needed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/divyagitech/Dataset-Practice.git
    cd Dataset-Practice
    ```

2. Open the notebook in Jupyter or Google Colab:
    - `EDA_Linear_Regression.ipynb`

3. Make sure the dataset is available at the specified path or update the code accordingly:
    ```python
    df = pd.read_csv("/path/to/Ecommerce Customers.csv")
    ```

4. Run the notebook cells step by step to follow the analysis and modeling.

## Key Steps in the Notebook

1. **Install and import libraries**  
   The notebook ensures all required libraries are installed and imported.

2. **Load the dataset**  
   Reads the CSV into a pandas DataFrame and displays the first few rows.

3. **Dataset overview and info**  
   Uses `.info()` and `.head()` to understand the structure and content.

4. **EDA and visualization**  
   - Joint plots for relationships (e.g., Time on Website vs Yearly Amount Spent)
   - Pair plots to visualize all relationships at once

5. **Feature selection and modeling**  
   - Selects numerical features for regression
   - Splits the data into training and test sets
   - Fits a linear regression model

6. **Model evaluation**  
   - Prints model coefficients
   - Evaluates model performance on the test data

## Results

The notebook provides:

- Visualizations of data relationships and distributions
- A trained linear regression model for predicting yearly customer spending
- Insights into which features drive customer spending

