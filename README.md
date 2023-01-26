# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd and import linear model from sklearn.

### Step2
Read the csv file.



### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fit.



### Step5
Print the predicted output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)               








```
## Output:

![Screenshot from 2023-01-26 15-25-25](https://user-images.githubusercontent.com/121165786/214807724-216e220a-7f58-4315-8d63-95efeeee2331.png)




## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
