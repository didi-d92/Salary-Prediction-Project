# Bank Marketing Campaign Analysis and Prediction
## Objective
The primary goal of this project is to predict whether a bank's client will subscribe to a term deposit after a marketing campaign. This analysis aims to understand the key factors influencing a client’s decision and to provide insights for more effective targeting in future campaigns.

## Dataset
The dataset used in this project includes various features related to the clients, such as age, job type, marital status, balance, contact details, previous marketing campaign outcomes, and the current campaign’s month and day. Some data preprocessing steps were required to handle missing values and convert categorical variables into numerical formats suitable for modeling.

## Key Steps in the Analysis
###### Data Exploration
- Loaded and examined the dataset’s structure, including the data types and unique values for each feature.
- Analyzed basic statistics and checked for any missing values or duplicates that could affect the modeling process.
###### Data Preprocessing
- Addressed missing values and encoded binary variables (e.g., yes/no to 1/0).
- Applied one-hot encoding to categorical variables like job type, education, and marital status.
- Scaled numerical features such as balance, duration, and campaign to normalize the data distribution and enhance model performance.
## Exploratory Data Analysis (EDA)
- Visualized the distribution of the target variable (deposit) to assess class balance.
- Identified relationships between the target variable and key features like duration, poutcome, and contact type.
- Created additional features to capture specific trends, such as a flag for December campaigns, due to observed seasonal peaks.
## Model Building
- Built a Logistic Regression model to predict whether a client would subscribe to the term deposit.
- Started with all available features, then refined the model by selecting the most significant predictors based on feature importance and correlation analysis.
- Evaluated the model using metrics like accuracy, precision, recall, and F1-score to assess its classification performance.
## Model Evaluation
- Cross-validated the model to ensure robustness and reduce overfitting.
- Analyzed results using confusion matrix, classification report, and key metrics:
Accuracy: 0.83 (or 83%)
Precision and Recall for each class (0 and 1):
Class 0: Precision 0.82, Recall 0.87, F1-score 0.84
Class 1: Precision 0.84, Recall 0.78, F1-score 0.81
Feature Importance
- Analyzed the coefficients from the Logistic Regression model to understand the impact of each feature:
duration had the highest positive influence, indicating that the length of a marketing call significantly increases the likelihood of subscription.
Other important factors included poutcome_success and contact_cellular.
## Results
The final model achieved an accuracy of 82.9%, with an F1-score of 0.83. The model's performance indicates that it can effectively predict client subscription based on the selected features, allowing for more targeted marketing efforts.

# Conclusion
This project demonstrated the effective use of Logistic Regression to predict client responses to marketing campaigns. The analysis provided valuable insights into the factors that influence client decisions, such as call duration and prior campaign outcomes.
