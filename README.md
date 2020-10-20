# Bank_Marketing_Campaign_Classification_Analysis

# Goal
Analyzed the prior marketing campaigns of a Portuguese Bank using various ML techniques like Logistic Regression, Random Forests, Decision Trees, Gradient Boosting and AdaBoost and predicted if the user will buy the Bank’s term deposit or not

# Software and Libraries Used
- Language: Python 
- Software: Jupyter Notebook
- Libraries: Pandas, Numpy, Matplotlib, Sklearn, Seaborn, Keras, Tensor Flow

# Description
- Bank Marketing dataset is collected from the direct marketing campaign of a bank institution from Portuguese. A marketing campaign can be understood as phone calls to the clients to convince them to accept to make a term deposit with their bank. After each call, they are being noted as to no - being the client did not make a deposit and yes - being the client on call accepted to make a deposit.

- The purpose of this project is to build an efficient classification model to predict if the client on-call would accept to make a term deposit or not based on the information of the clients.

Various Stages involved in this process are:
## 1. Data Cleaning
1. Understanding the data and imputing the missing values
2. Performed hot label encoding to categorical variables like a job, marital status, education, loan, housing,... columns.
3. Grouping the values in the columns age and duration together into categories as there are many unique values
 
## 2. Model Building
1. Splitting the data into train and test datasets using Sklearn packages
2. Building the following classification models:
   1. KNN Classification
   2. Logistic Regression
   3. Linear Support Vector Machine
   4. Kernelized Support Vector Machine (rbf, poly, and linear) 
   5. Decision Tree
  
3. Also applied ensembling modeling techniques 
   1. Random Forest
   2. Hard Voting
   3. Soft Voting
4. Applied Bagging Modeling Techniques on 
   1. Logistic Regression Model
   2. Random Forest Model
5. Applied Pasting Modeling Techniques on
   1. Kernelized_SVM 
   2. Decision Tree
6. Applied Adaboosting Modeling Techniques on
   1. Logistic Regression
   2. Random Forest
7. Gradient Boosting
8. Applied PCA to the data set and built the following models
   1. KNN Classification 
   2. Logistic Regression
   3. Linear Support Vector Machine
   4. Kernelized Support Vector Machine (rbf, poly, and linear) 
   5. Decision Tree
   6. Random Forest
9. Deep Learning  using Keras classifiers

** Performed grid search for tuning the hyperparameters and cross-validation for assessing the effectiveness of each of the above models. 
**  The results of the entire dataset are better for all models than the PCA models.

## 3. Model Selection     
- All the models are performing in a similar way his can be due to the reason that data may be clearly separated or can be classified using simple rules. For example, a decision tree with a depth of 4 is giving an accuracy of 91% with both train and validation.
- So for this problem, we look at other metrics such as AUC/ROC for model comparison. 

- ROC is visualized to select the best model. From ROC Curve, we see that random forest with adaptive boosting and random forest are the best. Ensemble methods are difficult to interpret. Therefore for the sake of interpretability, I'm choosing random forest as the top-performing model to predict if the user will buy the Bank’s term deposit or not.
