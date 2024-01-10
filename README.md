# NBA Player Salaries Analysis 

## Overview

This project focuses on analyzing NBA player salaries using R programming language. The primary goal is to understand the factors influencing player salaries and build predictive models to estimate salaries based on various player attributes and performance statistics.

## Project Structure

The project is organized into several sections:

1. **Data Loading and Cleaning:**
   - CSV files containing information about players and their salaries are loaded into R.
   - Player age, height, and weight are processed and transformed for better usability.

2. **Exploratory Data Analysis:**
   - Categorical variables are factorized for further analysis.
   - A subset of data for the year 2015 is created, and irrelevant columns are removed.

3. **Initial Model Fitting:**
   - An initial linear regression model (`lm`) is fitted without any feature selection or transformation.
   - Box-Cox transformation is applied to the dependent variable (salary) for better model fit.

4. **Feature Selection:**
   - Forward selection and backward elimination techniques are explored to identify significant features.
   - Subsequently, a reduced model with selected features is fitted.

   For regularization, L1 (Lasso) and L2 (Ridge) regularization can be applied. However, in this specific implementation, explicit regularization techniques are not demonstrated. To implement L1 and L2 regularization, the `glmnet` package can be utilized. Example code snippets are provided below:


   # L1 Regularization (Lasso)  and L2 Regularization (Ridge)
   `model_lasso = cv.glmnet(x, y, alpha = 1)`   alpha = 1 for Lasso

   `model_ridge = cv.glmnet(x, y, alpha = 0)`   alpha = 0 for Ridge


## Usage

To run the analysis, follow these steps:

1. Install required R packages by running the code in the ***Dependencies*** section.
2. Download and load the CSV files containing player and salary information from [https://data.world/datadavis/nba-salaries](https://data.world/datadavis/nba-salaries).
3. Execute each section of the R code sequentially.

## Results

The project results in predictive models for NBA player salaries, providing insights into the key factors influencing player compensation. Visualizations and statistical tests contribute to the overall understanding of the dataset.
Refer [Project_slides](https://github.com/patelvishwa1999/NBASalaryInsights/blob/d0408ba6064f534c40bda8e4bc8f174b96fb2af2/STAT%20596%20_%20Regression%20and%20Time%20Series%20Analysis%20FINAL%20PROJECT%20PRESENTATION.pdf) for more detailed results.

## Dependencies

`install.packages("installr")
installr::install.R()`

`install.packages("tidyverse")`

`install.packages("sqldf")`

`install.packages("MASS")`

`install.packages("glmnet")`
## Contributors

- Vishwa Patel
- Rutvik Despande
- Priyal Shaha
- Devyani Mardia

Feel free to reach out for any questions or contributions!
