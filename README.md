# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1
Import pandas library and linear_model from sklearn using import statement.
<br>

### Step2
Read the given csv file using read_csv().

<br>

### Step3
Create two arrays, independent array x withtwo classes and dependent array y with one class. Find the regression of x and y usimg linear_model.Linear Regression() method and fit x and y using.fit() method.
<br>

### Step4
Find the coefficients using coef_and intercept using intercept.

<br>

### Step5
Predict the linear regression using regr.predict9) method and display the result.
<br>


## Program:
```
import pandas as pd
from sklearn import linear_model

df  = pd.read_csv("cars.csv")
x = df[["Weight","Volume"]]
y = df["CO2"]
regr = linear_model.LinearRegression()
rregr.fit(x,y)

print("coefficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedco2=regr.predict([[3000,1200]])
print("Predicted co2 for the corresponding weight and volume ",predictedco2)
```
## Output:
```
coefficients: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted co2 for thr corresponding weight and volume [111.71387814]
```
## Insert your Output
![Screenshot (2022)](https://github.com/user-attachments/assets/9a16935f-ac4a-4084-9cab-fcc0058c8c85)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
