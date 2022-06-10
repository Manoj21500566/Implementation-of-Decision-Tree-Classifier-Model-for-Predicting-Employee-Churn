# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
~~~
1. Import the required libraries.
2.Upload and read the dataset.
3.Check for any null values using the isnull() function.
4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.
~~~


## Program:
```
/*

Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Manoj M 
RegisterNumber: 212221240027

import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evalution","number_project","average_montly_hours","time_spend_company","work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
Data Head:


![A1](https://user-images.githubusercontent.com/94588708/172999634-e5277459-e238-458e-9d2f-b6c75d28e644.png)

Information:


![A2](https://user-images.githubusercontent.com/94588708/172999716-340b5ebd-1005-4909-9a4a-e87b6fc2728f.png)


Null dataset:


![A3](https://user-images.githubusercontent.com/94588708/172999781-f023e802-927c-4262-a539-8e840518ee7a.png)

Value_counys():


![A4](https://user-images.githubusercontent.com/94588708/172999831-804e1f7f-f176-47e7-96fb-c6ab5671d70e.png)

Data Head:


![A5](https://user-images.githubusercontent.com/94588708/172999882-b34736bb-35fd-4741-a91f-a75d65f18e7e.png)

x.head():


![A6](https://user-images.githubusercontent.com/94588708/172999927-ff6ac057-849d-47c9-99fc-123a87ded6fe.png)


Accuracy:

![A7](https://user-images.githubusercontent.com/94588708/172999982-d7fb1aaa-074c-4762-bfa4-f72d5e0370e1.png)


Data Prediction:


![A8](https://user-images.githubusercontent.com/94588708/173000016-93552aa9-f72d-4c71-a07f-7d54d0312813.png)








## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
