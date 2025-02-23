# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Step1:
Get the independent variable X and dependent variable Y.
## Step2:
Calculate the mean of the X -values and the mean of the Y -values.
## Step3:
Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
## Step4:
Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
## Step5:
Use the slope m and the y -intercept to form the equation of the line.
## step6:
Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
# Univariate Linear Regression
# Develpoed by: MOHAMED AAKIF ASRAR S
# Register number: 23003613
import numpy as np
import matplotlib.pyplot as plt
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean=np.mean(x)
ymean=np.mean(y)
num=0
den=0
for i in range(len(x)):
num+=(x[i]-xmean)*(y[i]-ymean)
den+=(x[i]-xmean) **2
m=num/den
b=ymean-m*xmean
print(m,b)
ypred=m*x+b
print(ypred)
plt.scatter(x,y,color="Red")
plt.plot(x,ypred, color="Blue")
plt.show()

```
## Output
![Screenshot 2023-12-28 175919](https://github.com/MOHAMEDAAKIFASRAR/Univariate-Linear-Regression/assets/148514683/997a282b-ed9c-47d8-9e6f-73c1037177ab)
![Screenshot 2023-12-28 175851](https://github.com/MOHAMEDAAKIFASRAR/Univariate-Linear-Regression/assets/148514683/191567f4-8a10-4124-9a21-3a90e78979dd)

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
