# Customer-Conversion-Prediction-on-New-Age-insurance-Data
# Problem Statement
You are working for a new-age insurance company and employ mutiple outreach plans to sell term insurance to your customers. Telephonic marketing campaigns still remain one of the most effective way to reach out to people however they incur a lot of cost. Hence, it is important to identify the customers that are most likely to convert beforehand so that they can be specifically targeted via call. We are given the historical marketing data of the insurance company and are required to build a ML model that will predict if a client will subscribe to the insurance.
# Features:
age (numeric)
job : type of job
marital : marital status
educational_qual : education status
call_type : contact communication type
day: last contact day of the month (numeric)
mon: last contact month of year
dur: last contact duration, in seconds (numeric)
num_calls: number of contacts performed during this campaign and for this client
prev_outcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")

# Output variable (desired target):
y - has the client subscribed to the insurance?

# Insights from Problem Statement and Features::
After Reading the Problem Statement & Going through the Features ,column by column in a data set, we can Say this is a Supervised Learning Problem With Classification Model of Binary Subset Classification(Y/N)

# Insights from Data Preprocessing :

After Data Cleaning process with removing Duplicates , handling unknown Values & Outlier detection 
Checking our Target Varaiable
Percentage for "no":  88.29996681782988
Percentage for "yes":  11.700033182170113

Hence Our Data is Imbalanced So We Need to Balance the data & Then Need to Scale & Split the Data 

# Models Implemented for Supervised binary Classification Problem:

Logistic Regression 
KNN 
Decision Tree
XG Boost - AUROC Score 
Random Forest - AUROC Score

# Solution Statement
Models are tested, below are the AUROC value of each model

Logistic Regression - AUROC Score is 0.90
KNN - AUROC Score is 0.805
Decision Tree - AUROC Score is 0.786
XG Boost - AUROC Score is 0.904
Random Forest - AUROC Score is 0.9036
Hence XGboost is giving the good AUROC Score of 0.904, so XGboost is the best model for customer convertion prediction
