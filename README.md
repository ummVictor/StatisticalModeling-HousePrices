# StatisticalModeling-HousePrices

https://www.kaggle.com/c/house-prices-advanced-regression-techniques

---

## Project Overview

This project aims to predict house prices using a dataset with 81 features, leveraging regression and machine learning techniques. Key deliverables included cleaning and enriching data, exploring feature relationships, building predictive models, and evaluating model performance against the Kaggle benchmark.

**Dataset Components:**

- `train.csv`: Training dataset with 1,460 entries and 81 features.
- `test.csv`: Test dataset for predictions.
- `data_description.txt`: Detailed explanation of dataset columns.
- `sample_submission.csv`: Example submission with basic predictions.

---

## Features and Methodology

### 1. Data Cleaning

- **Handling Missing Values:**
  - Imputed medians for numeric data.
  - Assigned "None" for missing categorical data.
- **Outlier Detection and Removal:** Used scatterplots and domain knowledge.
- **Categorical Encoding:** Converted string categories into factors for modeling.

### 2. Exploratory Data Analysis (EDA)

- **Visualizations:**
  - Distribution of `SalePrice` with histograms.
  - Scatterplots for key relationships (e.g., `GrLivArea` vs. `SalePrice`).
- **Feature Analysis:** Identified top predictors like `TotalSqFt` and `OverallQual`.

### 3. Data Enrichment

- **Log-Transformation:** Stabilized variance of `SalePrice`.
- **New Features:**
  - `TotalSqFt` combining ground living area and basement area.
- **Feature Selection:** Focused on meaningful predictors using LASSO regression.

### 4. Modeling

- **Techniques Applied:**
  - LASSO Regression: Regularization and feature selection.
  - Ridge Regression: Addressed multicollinearity.
  - Gradient Boosting: Enhanced predictive accuracy.
- **Validation Strategy:**
  - Used an 80/20 train-test split for cross-validation.
  - Evaluated models using RMSE on log-transformed `SalePrice`.

### 5. Evaluation

- **Metrics:**
  - Root Mean Square Error (RMSE): Standard metric for Kaggle submissions.
  - RMSE on log-transformed prices: **0.0904**.
- **Insights:**
  - LASSO regression effectively selected relevant features, reducing overfitting.
  - Log-transformation of `SalePrice` improved model performance.

---

## Results

The project tackled challenges like missing data, heteroscedasticity, and high dimensionality. Using advanced modeling techniques and thorough feature engineering, we developed a robust predictive model with competitive accuracy.

**Key Achievements:**

- Effective handling of 81 features and imbalanced data.
- Successful application of LASSO regression for feature selection.
- Strong performance with RMSE of **0.0904** on the log-transformed target.

---

## Files

- `train.csv`: Training dataset.
- `test.csv`: Test dataset.
- `data_description.txt`: Feature descriptions and explanations.
- `sample_submission.csv`: Example Kaggle submission with predictions based on a basic linear regression model.

---

## Conclusion

This project demonstrated the power of data science techniques in solving real-world regression problems. By combining EDA, feature engineering, and machine learning, we achieved a high-performing model. The process also highlighted the importance of addressing data issues like missing values and feature scaling in predictive analytics.
