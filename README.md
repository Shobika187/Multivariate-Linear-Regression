# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

we find multi varient linear regtrssion using pandas.

### Step2

we find from sklearn import linear model.

### Step3

First we have to read a file using pandas.

### Step4

In this programm we take u variables weight and volume.

### Step5

Using this two variables we find coefficient and interscept.

## Program:
```
##Name : P Shobika
##Reg No: 212221230096
import pandas as pd 
from sklearn import linear_model
df = pd.read_csv("cars.csv")

x = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(x, y)

print('Coefficients: ',regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2 = regr.predict([[3300, 1300]])
print('predicted CO2 for the corresponding Weight and Volume',predictedCO2)






```
## Output:
![GitHub Logo](.//img3.png)


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
