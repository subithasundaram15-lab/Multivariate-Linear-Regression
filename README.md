# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1
Import the required libraries: pandas for data manipulation and linear_model from sklearn for regression

### Step2
Load the dataset using pd.read_csv() and store it in a DataFrame

### Step3
Separate the features (independent variables) and the target (dependent variable):

Assign the relevant columns to X (features). Assign the target column to y (output)

### Step4
Separate the features (independent variables) and the target (dependent variable):

Assign the relevant columns to X (features). Assign the target column to y (output)

### Step5
Print the regression coefficients (regr.coef_) and intercept (regr.intercept_)

### Step6
Use the trained model to make predictions using regr.predict() with the given input values.

### Step7
Display the predicted output.

## Program:
```
Developed by: SUBITHA S
RegisterNumber: 212225040432

import pandas as pd
from sklearn import linear_model

df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)

```
## Output:

<img width="1043" height="129" alt="image" src="https://github.com/user-attachments/assets/7d61fb97-3ac2-4154-919c-f998aac1a3a2" />

## Result

Thus the multivariate linear regression is implemented and predicted the output using python program.
