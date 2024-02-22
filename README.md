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
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: santhosh kumar B
RegisterNumber: 212223230193 
*/
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.metrics import mean_absolute_error,mean_squared_error
df = pd.read_csv("./content/student_marks.csv")
df.head()
plt.scatter(df["X"],df["Y"])
plt.xlabel("X")
plt.ylabel("y")
X = df.iloc[:,:-1].values
X
Y = df.iloc[:,1].values
Y
from sklearn.model_selection import train_test_split
X_train,X_test,Y_train,Y_test = train_test_split(X,Y,test_size=0.2,random_state=0)
from sklearn.linear_model import LinearRegression
lr = LinearRegression()
lr.fit(X_train,Y_train)
plt.scatter(df["X"],df["Y"])
plt.xlabel("X")
plt.ylabel("Y")
plt.plot(X_train,lr.predict(X_train),color="red");
```

## Output:
![image 2024-02-22 131809  1](https://github.com/Santhoshstudent/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/145446853/8f3b4cab-c3c6-4549-84b5-f9ac20099845)
![image 2024-02-22 132013 2](https://github.com/Santhoshstudent/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/145446853/55fd0cd2-fff9-48cf-81f1-79a5c3ff9733)
![image 2024-02-22 132129 3](https://github.com/Santhoshstudent/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/145446853/dd815025-6797-4d61-baa5-957101fd0ce6)
![image 2024-02-22 132337 5](https://github.com/Santhoshstudent/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/145446853/66e0893a-b5bd-40b8-b020-d2753f2e1403)
![image 2024-02-22 132615 6](https://github.com/Santhoshstudent/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/145446853/aece16bf-edc3-4b63-b6b0-5f4eed027995)
![image 2024-02-22 132704 7](https://github.com/Santhoshstudent/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/145446853/7a3b759c-80a7-465c-9606-61ca7364c19f)
![image 2024-02-22 132802 7](https://github.com/Santhoshstudent/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/145446853/b2f27566-999e-40d8-9133-74f2613f10f6)
![image 2024-02-22 132905 8](https://github.com/Santhoshstudent/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/145446853/4e1ef250-3162-4942-84a6-6c7cf13ad76d)










## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
