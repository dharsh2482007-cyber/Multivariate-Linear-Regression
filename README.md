# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

##Step1

Import the required libraries such as pandas and sklearn linear model.

##Step2

Read the dataset file using pandas read_csv() function.

##Step3

Store the independent variables (Volume, Weight) in x and dependent variable (CO2) in y.

##Step4

Create a Linear Regression model and train the model using fit() method.

##Step5

Predict the CO2 emission value using predict() method and display the coefficients, intercept, and predicted output.
## Program:
```


#DEVELOPED BY : P.PRIYADHARSHINI
#REGISTER NUMBER :212225220076

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))



```
## Output:

[0.00780526 0.00755095]

79.6947192911594

[115.26830058]

### Insert your output

<img width="1917" height="1077" alt="image" src="https://github.com/user-attachments/assets/e4474066-08e7-45b6-89d1-be55eba89cd5" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
