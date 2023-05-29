# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas

### Step2
import linear model

### Step3
Read the csv file

### Step4
Enter the parameters to implement

### Step5
Run the program and predict the output

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print("Intercept",regr.intercept_)
predictedCO2=regr.predict([[1995,522]])
print("Predicted CO2 emission based on weight")
```
## Output:
![image](https://github.com/Pravinrajj/Multivariate-Linear-Regression/assets/117917674/d085a5ce-a2f8-4460-96c6-a16b2806be77)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
