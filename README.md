# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## STEP 1:
 Get the independent variable X and the dependent variable Y.
## STEP 2:
 Calculate the mean of the X -values and the mean of the Y -values.
## STEP 3
 Find the slope m of the line of best fit using the formula.![eqn1](./eq1.jpg)
## STEP 4:
 Compute the y-intercept of the line by using the formula:![eqn2](./eq2.jpg) 
## STEP 5:
 Use the slope m and the y-intercept to form the equation of the line.
## STEP 6:
 Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: SREEKUMAR S
Register number:23008070

import numpy as np
import matplotlib.pyplot as py
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num,num1=0,0
for i in range(len(x)):
  num+=(x[i]-x_mean)*(y[i]-y_mean)
  num1+=(x[i]-x_mean)**2
m=num/num1
b=y_mean-(m*x_mean)
print(m,b) 
y_pred=(m*x)+b
print(y_pred)
py.scatter(x,y,color='blue')
py.plot(x,y_pred,color="#CD5555")
py.show()
```
## Output
![Screenshot 2023-12-24 195542](https://github.com/guru14789/Univariate-Linear-Regression/assets/151705853/507173c0-b187-4114-b49a-038e1ecf617b)

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
