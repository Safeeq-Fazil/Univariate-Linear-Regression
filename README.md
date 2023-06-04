# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.


![exp 9 step 3](https://github.com/Safeeq-Fazil/Univariate-Linear-Regression/assets/118680361/22425bb6-3a30-4970-8239-782bf093eba2)


4.	Compute the y -intercept of the line by using the formula:



![exp 9 step 4](https://github.com/Safeeq-Fazil/Univariate-Linear-Regression/assets/118680361/5584f4ca-2118-430b-9e71-1ba59e748108)

5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```

Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Safeeq Fazil.A
Register number: 212222240086
import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
xmean=np.mean(x)
ymean=np.mean(y)
num,den=0,0
for i in range(len(x)):
  num+=(x[i]-xmean)*(y[i]-ymean)
  den+=(x[i]-xmean)**2
m=num/den
c=ymean-m*xmean
print(m,c)
y_pred=m*x+c
print(y_pred)
plt.scatter(x,y)
plt.plot(x,y_pred,color="orange")
plt.show()






```
## Output
![exp 9](https://github.com/Safeeq-Fazil/Univariate-Linear-Regression/assets/118680361/13e2bece-97a2-4aa5-8e2d-3768f4ff1cd9)


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
