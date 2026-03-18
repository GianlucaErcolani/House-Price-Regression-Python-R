# House Price Advanced Regression project

This project explores the factors influencing residential property prices and builds predictive models using advanced regression techniques. The unique value of this repository is the **dual-language approach**: using **Python** for Exploratory Data Analysis (EDA) and data cleaning, and **R** for specialized statistical modeling like Ridge and Lasso regression.

### Project Structure

* `House_price_Part1.py`: Python script focused on:
    * **Exploratory Data Analysis (EDA)**: Visualizing distributions and identifying strong correlations (e.g., SalePrice vs. GrLivArea).
    * **Data Cleaning**: Systematic handling of missing values and feature selection.
    * **Preprocessing**: Converting categorical variables into dummy variables for modeling.
* `House_price_Part2.R`: R script focused on:
    * **Advanced Statistical Modeling**: Implementation of **Ridge Regression** and **Lasso Regression**.
    * **Hyperparameter Tuning**: Using cross-validation (`cv.glmnet`) to find the optimal lambda value.
    * **Model Comparison**: Evaluating Mean Squared Error (MSE) across different regression approaches.
* `requirements.txt`: Python library dependencies.



### Dataset

The analysis is performed on the popular House Prices dataset, containing 79 explanatory variables describing almost every aspect of residential homes.

**Key Features Analyzed:**
* `SalePrice`: The target variable (price in dollars).
* `GrLivArea`: Above grade (ground) living area square feet.
* `OverallQual`: Rates the overall material and finish of the house.
* `TotalBsmtSF`: Total square feet of basement area.
* `YearBuilt`: Original construction date.

### Results
* **EDA Insights**: Identified a strong positive linear relationship between `GrLivArea` and `SalePrice`, as well as high correlations with `OverallQual` and `TotalBsmtSF`.
* **Model Performance**: The R-based Lasso model provided an efficient feature selection mechanism, while the Ridge model's optimal lambda was determined via cross-validation to minimize prediction error.
