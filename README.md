# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1
Get the independent variable X and dependent variable Y.
<br>

### Step2
Calculate the mean of the X -values and the mean of the Y -values.
Find the slope m of the line of best fit using the formula. 
![eq1](https://github.com/user-attachments/assets/7ce2564b-6871-4cf7-aa56-d13529fec172)

<br>

### Step3
Find the slope m of the line of best fit using the formula. 
![eq2](https://github.com/user-attachments/assets/d6722ce5-6898-4cf3-a992-0aa49ea5d37c)

<br>

### Step4
Compute the y -intercept of the line by using the formula: 

<br>

### Step5
Use the slope m and the y -intercept to form the equation of the line.
<br

### Step6
Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
import numpy as np 
import matplotlib.pyplot as plt
x = np.array([0,1,2,3,4,5,6,7,8,9])
y = np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean = np.mean(x)
ymean = np.mean(y)
num=0
den=0
for i in range(len(x)):
    num+=(x[i]-xmean)*(y[i]-ymean)
    den+=(x[i]-xmean)**2
m = num/den
b = ymean - m*xmean
print(m,b)
ypred = m*x+b
print(ypred)

plt.scatter(x,y,color='Red')
plt.plot(x,ypred,color='Blue')
plt.show()
```
## Output:
![practical](https://github.com/user-attachments/assets/8d646808-c526-4f25-8cbd-c6bc82b67926)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
