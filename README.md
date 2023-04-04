# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: YUGENDARAN.G
RegisterNumber:  212221220063

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.metrics import mean_absolute_error,mean_squared_error
df=pd.read_csv('/content/student_scores.csv')
#displaying the content in datafile
[1] print("df.head():")
    df.head()

[2] print("df.tail(): ")
    df.tail()
  
[3] print("Array values of x:")
    x=df.iloc[:,:-1].values
    x
    
[4] print("Array value of y:")
    y=df.iloc[:,1].values
    
[5] #splitting train and test data
    from sklearn.model_selection import train_test_split
    x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=1/3,random_state=0)
    
    from sklearn.linear_model import LinearRegression
    regressor=LinearRegression()
    regressor.fit(x_train,y_train)
    y_pred=regressor.predict(x_test)
    
    #displaying predicted values
    y_pred
    
```
## Output:
![image](https://user-images.githubusercontent.com/128135616/229407897-6118d22a-60ea-46f8-9122-3eb02f3fcd21.png)

![image](https://user-images.githubusercontent.com/128135616/229409013-8619da20-1224-4018-b95b-0d74e22e950f.png)

![image](https://user-images.githubusercontent.com/128135616/229409927-c29886cf-7bc0-4fa2-9d62-3e0bf51b3b97.png)

![image](https://user-images.githubusercontent.com/128135616/229430829-372414ea-f6cb-438b-8762-92dd0ecc0cba.png)

![image](https://user-images.githubusercontent.com/128135616/229709402-08c04449-7e71-4ad7-9a9e-121d73330810.png)











## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
