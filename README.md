# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step 1: Select the features. First, you need to select that one feature that drives the multivariate regression. ...

Step 2: Normalize the feature. ...

Step 3: Select loss function and formulate a hypothesis. ...

Step 4: Minimize the cost and loss function. ...

Step 5: Test the hypothesis.


## Program:
```
import pandas as pd

from sklearn import linear_model

df = pd.read_csv("C:\\Users\\admin\\Downloads\\car.csv")

X = df[['Weight', 'Volume']]

y = df['CO2']

regr = linear_model.LinearRegression()

regr.fit(X, y)

print('Coefficients:', regr.coef_)

print('Intercept:',regr.intercept_)

predictedCO2 = regr.predict([[3300, 1300]])

print('Predicted CO2 for the corresponding weight and volume',predictedCO2)






```
## Output:

### Insert your output

![Screenshot 2024-12-06 014115](https://github.com/user-attachments/assets/d87f98f3-d46e-4905-89e3-34ca214a2e1e)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
