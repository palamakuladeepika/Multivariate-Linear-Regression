# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:
Import Pandas module

### Step 2:
Read the csv file.

### Step 3:
Get the values of X and Y variable.

### Step 4:
Create the linear regression and fit.

### Step 5:
Predict CO2 with appropriate values.

### Step 6:
Display the predicted value.

## Program:
```
~~~
#Developed by :- P.Deepika
#Reference number:- 212221240035
~~~
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('cars.csv')
X = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X,y)
print("Cofficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedCO2 = regr.predict([[3300,1300]])
print('Predicted co2 for the corresponding weight and volume',predictedCO2)

```
## Output:
![output](carsdeepika.png)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
