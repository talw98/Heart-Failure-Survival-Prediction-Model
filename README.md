# Heart-Failure-Prediction-Model
*Building a Machine Learning Model utilizing Logistic Regression to predict death from Heart Failure.*

# Background

Heart Failure is one of the most widespread medical emergencies in the world and a cause of large number of deaths in the global population. In this project, Machine Learning will be used to predict whether a patient with heart failure dies or not based on the ejection fraction of their heart and serum creatinine levels. Since the result will be a binary classification (Dead i.e, 1 or Alive i.e, 0), Logistic Regression will be used to predict whether the patient with heart failure will die or not.

# Dataset
The dataset for this model is obtained from [Kaggle](https://www.kaggle.com/datasets/andrewmvd/heart-failure-clinical-data). The dataset has 13 columns and a total of 299 rows. The columns are **Age, Anaemia, Creatinine Phosphokinase, Diabetes, Ejection Fraction, High Blood Pressure, Platelets, Serum Creatinine, Serum Sodium, Sex, Smoking, Time and Death Event.**

# Data Pre processing
The datset is cleaned by dropping all the null values if they were present. Requisite libraries such as *Pandas, Numpy* and *Scikit-Learn* were imported. Only two columns, **Ejection Fraction** and **Serum Creatinine** were used and the rest were dropped. The reason why Ejection Fraction and Serum Creatinine were selected is because these two features alone can lead to more accurate predictions than using the original dataset features in its entirety, according to a research published in the [BMC Journal.](https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/s12911-020-1023-5)

# Model Training
The machine learning model utilises the Logistic Regression algorithm to predict whether heart failure patient will survive or not. 70% of the data is used to train the model and the remaining 30% is categorised as testing data. This split is done bt the train_test_split function imported from scikitlearn. A logistic regression model is then instantiated and fit to the training data using the 'fit' method. The coefficients and intercept of the logistic regression model are printed and the model is then used to predict the outcome of new data using the 'predict' method.

# Conclusion
In conclusion, this project provides a comprehensive overview of the heart failure clinical records dataset and prepares the data for training and testing. The machine learning model based on logistic regression can predict whether a patient will survive from heart failure or not. This approach may assist medical professionals in early detection and management of heart failure. 
