@AUTHOR : Sarang Bagul

# Bank-Marketing-Classification
This project utilizes different types of Machine Learning algorithm, using the Bank Marketing dataset, to check if the client has subscribed for a term deposit depending on various bank marketing attributes like age, type of job, education level, if the client has housing loan or not, last date of contact etc.

DATA PREPROCESSING :
1. As there are no missing values. So we randomly replace values by NaN. We fill values by mean/median/mode.
2. Done EDA to get insigts from the data as :
   a. count plot of categorical data
   b. Histogram of Numerical data to check distribution of the data
3. Transform categorical feature values to numeric type for model building
   a. LabelEncoding
   b. One Hot Encoding for features more than two values
4. MinMax Scaler to scale data to one range for faster processing
5. Train and Test Split
6. As data is imbalance. So balance TRAINING DATA using SMOTE

Model Building :
1. Fitted following models on default values:
   a. Logistic Regression
   b. SVM
   c. Decision TreeClassifier
   d. Random Forest
   e. AdaBoost
2. Tune hyper-parameter of the model which gives best result on default model.

Evaluation Metrices:
1. For this problem statement, Recall is more important metric. As people actually subscribed but predicted as not subscribe (Type - II error)
   So recall should be high as possible. As More cost is associated with Type-II error.
