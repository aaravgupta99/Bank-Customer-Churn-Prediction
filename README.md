
# Bank Customer Churn Prediction Project - Readme
## Overview
This data science project aims to build a predictive model for identifying bank customers likely to churn. Customer churn refers to the situation where a customer stops using the services of a company. In this case, churn means customers who leave the bank. By predicting potential churners, the bank can take proactive measures to retain these customers and minimize customer attrition.
## Dataset

 - [Bank Customer Churn Dataset](https://www.kaggle.com/datasets/adammaus/predicting-churn-for-bank-customers)

The dataset used in this project is named "Churn_Modelling.csv," obtained from Kaggle. It is a CSV file that contains customer information and churn status for a bank. The dataset includes the following attributes:

RowNumber: The row number in the dataset.
CustomerId: Unique identifier for each customer.
Surname: Customer's surname (last name).
CreditScore: Customer's credit score.
Geography: Customer's geographical location (country).
Gender: Customer's gender (Male or Female).
Age: Customer's age.
Tenure: Number of years the customer has been with the bank.
Balance: Bank account balance.
NumOfProducts: Number of bank products the customer has purchased.
HasCrCard: Whether the customer has a credit card (0 = No, 1 = Yes).
IsActiveMember: Whether the customer is an active member (0 = No, 1 = Yes).
EstimatedSalary: Estimated salary of the customer.
Exited: Whether the customer has churned (0 = No, 1 = Yes).
## Packages Used

The following Python packages were used in this project:

1. pandas: For data manipulation and analysis.
2. sklearn: For various machine learning algorithms and evaluation metrics.
3. tensorflow: For building and training deep learning models.
4. matplotlib, seaborn: For data visualization and exploration.
5. imblearn: For handling the imbalanced nature of the data.
## Project Steps

### Importing Dependencies:
Modules, packages, classes, functions necessary for the project are imported.

### Data Preprocessing: 
The first step involves loading the dataset and performing necessary data cleaning and transformations to prepare the data for analysis. Since the data is imbalanced, the imblearn package is used to address this issue.

### Exploratory Data Analysis (EDA): 
In this step, the dataset is analyzed to gain insights into the relationship between customer attributes and churn status. Various visualizations and statistical summaries are used to explore the data and identify patterns or trends that can help in building the predictive model.

### Feature Engineering: 
Feature engineering is an essential part of building a successful predictive model. It involves transforming features to enhance the model's predictive power. In this project, relevant features will be selected, and new features may be created if necessary.

### Dealing with imbalanced data:
0 class:    7963

1 class:   2037

The data is imbalanced. Training the data as it is may result in overfitting. 
imblearn.undersampling.NearMiss class is used for dealing with the issue.

### Model Fitting and Selection: 
The main focus of this project is on building a deep neural network to predict customer churn.

### Model Evaluation: 
The performance of the deep neural network model is evaluated using appropriate evaluation metrics, such as accuracy, precision, recall, and F1 score.

### Test Data Prediction:
The final trained deep neural network model is applied to unseen test data to evaluate its performance on new observations. The metrics calculated during this step provide insights into the model's generalization ability.


## Conclusion
By developing an accurate churn prediction model using a deep neural network, the bank can proactively identify customers at risk of churn and implement targeted retention strategies to maintain a strong customer base and improve overall business performance. The successful implementation of the deep neural network demonstrates the significance of data science in making informed business decisions and optimizing customer retention strategies.