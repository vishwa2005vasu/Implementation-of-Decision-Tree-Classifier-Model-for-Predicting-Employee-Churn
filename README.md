# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

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
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Vishwa vasu. R 
RegisterNumber:212222040183
import pandas as pd
data=pd.read_csv("/content/Employee.csv")

print('data.info:')
data.info()

print('data.isnull().sum():')
data.isnull().sum()

print('value_count: ')
data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()

data["salary"]=le.fit_transform(data["salary"])
data.head()

*x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()**

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
![Screenshot 2023-10-12 092325](https://github.com/vishwa2005vasu/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135954202/9d4b39ae-1757-4e88-b700-e2096986bcb5)
![Screenshot 2023-10-12 092854](https://github.com/vishwa2005vasu/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135954202/36930628-0377-4d86-b672-d27c049ba210)
![Screenshot 2023-10-12 092956](https://github.com/vishwa2005vasu/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135954202/68a315d1-5698-4316-a11e-8a9298c76a4e)
![Screenshot 2023-10-12 093249](https://github.com/vishwa2005vasu/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135954202/9d090944-4f84-4b75-b8e1-3bfb7b9a0662)
![Screenshot 2023-10-12 093304](https://github.com/vishwa2005vasu/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135954202/ccb4d6fc-ef10-4723-92d3-2f240a5f4d1c)
![Screenshot 2023-10-12 093318](https://github.com/vishwa2005vasu/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135954202/b6f2d354-1222-4732-9254-d8cb0774fbf2)
![Screenshot 2023-10-12 093334](https://github.com/vishwa2005vasu/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135954202/c7b5e17c-f5d9-4dfb-a631-749082fbcf82)
![Screenshot 2023-10-12 093352](https://github.com/vishwa2005vasu/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135954202/7a4ca842-6107-415d-a0f3-6215fce217b4)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
