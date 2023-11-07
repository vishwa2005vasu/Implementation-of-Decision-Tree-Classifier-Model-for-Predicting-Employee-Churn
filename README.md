# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Start the program
2.Import the python pandas library as pd
3.Read the dataset of Employee csv file
4.Display the data information using info() method
5.Import the LabelEncoder for preprocessing of the dataset
6.Assign the columns for x and y
7.From sklearn library import the Decision Tree Classifier to predict the values
8.Print the accuracy of the dataset
9.Predict the decision tree using random values
10.Stop the program

## Program:
```
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

x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()

y=data["left"]

from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(x,y,test_size=0.2, random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test, y_pred)
accuracy

dt.predict([[0.5, 0.8, 9, 260, 6, 0, 1, 2]])

Developed By :L.Mahesh Muthu
Register Number:212222040093

```

## Output:


 1.Initial data set


 

![Screenshot (69)](https://github.com/MaheshMuthuL/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135570619/7d517752-acf3-467d-b3bc-87cfe646e705)






2. Data Info






![Screenshot (70)](https://github.com/MaheshMuthuL/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135570619/abf43f26-9ba0-432c-8dc2-2f70f59a5f94)





3. Optimization of null values





![Screenshot (71)](https://github.com/MaheshMuthuL/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135570619/4b51b1b1-2d3b-491e-8c36-70cbffed80df)






4.Assignment of X and Y values





![Screenshot (72)](https://github.com/MaheshMuthuL/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135570619/f3654906-27d2-4ae7-bd48-534e79b40ddb)





5.Converting string literals to numerical values using label encoder





![Screenshot (73)](https://github.com/MaheshMuthuL/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135570619/a06a5d4d-1939-4417-9fae-a707a3860057)




6. Accuracy





![Screenshot (74)](https://github.com/MaheshMuthuL/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135570619/f722f0e0-927a-4795-b9d0-41cc6a79e9ff)






7. Prediction




![Screenshot (75)](https://github.com/MaheshMuthuL/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135570619/1fb54cd8-b8ec-40d8-94a3-644a4c3ebe45)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
