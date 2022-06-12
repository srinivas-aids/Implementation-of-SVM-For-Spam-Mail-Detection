# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Import the required packages.
2.Import the dataset to operate on.
3.Split the dataset.
4.Predict the required output.
5.End the program

## Program:
```
~~~
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: u.srinivas
RegisterNumber:  212221230108
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Manoj M
RegisterNumber:  212221240027
import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extractiaon.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
~~~
*/
```

## Output:
## DATA HEAD:


![1](https://user-images.githubusercontent.com/93427183/173223434-75198e20-5bae-4091-b84e-5bf95da7abf8.png)


## DATA INFO:


![2](https://user-images.githubusercontent.com/93427183/173223442-f0e1174a-394c-49a1-9c64-bda6c2ba32e0.png)


## Data isnull():


![3](https://user-images.githubusercontent.com/93427183/173223451-46196de2-5e89-4491-9f9c-efb88bf8a101.png)


## y_pred:



![4](https://user-images.githubusercontent.com/93427183/173223461-85d2efa8-fcac-467b-be51-02505239fe3c.png)

## Accuracy:


![173184122-47c59aa7-86b2-4a41-b672-efe4985fa0d5](https://user-images.githubusercontent.com/93427183/173223466-e020ccab-9184-4a7e-bf59-7d0785014776.png)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
