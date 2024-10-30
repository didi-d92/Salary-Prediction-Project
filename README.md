# Salary Prediction
## Objective
The primary goal of this project is to predict the salary of individuals based on specific criteria available in the dataset. This analysis aims to understand the factors influencing salary levels and provide insights for fair compensation practices.

## Dataset
The dataset used in this project is Salary_Data.csv, which contains information on various job titles, education levels, years of experience, age, and gender. The dataset may have missing values that need to be addressed before performing any analysis or modeling.

## Key Steps in the Analysis
### Data Exploration
Loaded the dataset and examined its structure. Analyzed basic statistics and checked for missing values and duplicates.
### Data Preprocessing
Handled missing values using KNN imputation for numerical data. Filled categorical variables using the mode for missing entries. Converted categorical variables (e.g., Job Title, Education Level) into numerical representations using one-hot encoding.

## Exploratory Data Analysis (EDA)
Visualized salary distributions and identified outliers. Investigated relationships between salary and other factors such as job title, education level, and years of experience.

## Model Building
Created multiple linear regression models to predict salaries. Initially included all available features and later refined the model by selecting key predictors based on correlation analysis. Evaluated model performance using metrics such as R² and Mean Squared Error (MSE).

## Model Evaluation
Analyzed overfitting using RMSE for training and testing datasets. Applied cross-validation to ensure model robustness.

## Results
The final model achieved an R² score of approximately 0.69, indicating that about 69% of the variance in salary can be explained by the selected features. Predictions were plotted against actual salary values to visualize model performance.

## Conclusion
This project successfully demonstrated how to predict salaries based on various features, allowing for insights into compensation practices. While the linear regression model provided a solid baseline, further exploration with other modeling techniques could enhance predictive accuracy.
