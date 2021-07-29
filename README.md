# **Risky-Business**
---
![Risk](Images/credit-risk.jpeg)

---
## **Background**

Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, it imperative to predict and control credit risk.

---
## **Objective**
The objective is to  build and evaluate several machine learning models to predict credit risk using data sourced from  peer-to-peer lending services. 

Credit risk is an inherently imbalanced classification problem i.e the number of standard loans is far exceed than the number of at-risk loans. Hence we need to employ different techniques for training and evaluating models with imbalanced classes. 

---
## **Steps**


A.  **Resampling**

1. Read the LendingClub data stored in CSV files into a Pandas DataFrame.

2. Split the data into Training and Testing sets using `train_test_split`

3. Scale the training and testing data using the `StandardScaler` from `sklearn.preprocessing`.

4. Run a Simple Logistic Regression and calculate `balanced accuracy score`, display the `confusion matrix` & `imbalanced classification report`.


5. To handle the problem of imbalanced classes, 
    * Oversample the data using the `Naive Random Oversampler` and `SMOTE` algorithms. usion matrix` & `imbalanced classification report`.

    *  Undersample the data using the `Cluster Centroids` algorithm.

    * Over- and undersample using a combination `SMOTEENN` algorithm.
    
    For each of the above

    * Apply a Logistic Regression Model and calculate the `balanced accuracy score` from `sklearn.metrics`.Display the `confusion matrix` from `sklearn.metrics` and  `imbalanced classification report` from `imblearn.metrics`.

6. Evaluate the results 

B. **Ensemble Learning**

1. Read the loand data into a Pandas DataFrame 

2. Split the data into training and testing sets using `train_test_split`

3. Scale the training and testing data using the `StandardScaler` from `sklearn.preprocessing`.

4. Apply `Balanced Random Forest Classifier` and `Easy Ensemble Classifier` models to the training data. Calculate `balanced acurracy score`, `confusion matrix` from `sklearn.metrics` & `classification report` using the imbalanced learn.

5. For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.



---
## **Technologies/Tools/Libraries**
 1. Python
 2. Pandas
 3. Matplotlib
 4. Numpy
 5. Path
 6. sklearn.preprocessing
 7. sklearn.linear_model
 8. sklearn.metrics
 9. imblearn.over_sampling
 10. imblearn.under_sampling
 11. imblearn.metrics
 12. imblearn.combine
 11. Collections
 12. Jupyter Notebook

---
## **Data**
* [Lending Club Loans Data](Resources/LoanStats_2019Q1.csv)
* [Lending Data](Resources/lending_data.csv)

---
## **Code**
* [Resampling](credit_risk_resampling.ipynb)
* [Esemble](credit_risk_ensemble.ipynb)


