# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
import pandas as pd
<br>
### Step2:
Read the csv file.
<br>
### Step3:
Get the value of X and y variables.
<br>
### Step4:
Create the linear regression model and fit.
<br>
### Step5:
predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3.
<br>
### Step6:
Print the predicted output.

## Program:
```python
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:
![image](https://github.com/sanjeevi00/Multivariate-Linear-Regression/assets/121484976/f81b0648-5e31-4962-8623-e7a1ed8e3d37)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
