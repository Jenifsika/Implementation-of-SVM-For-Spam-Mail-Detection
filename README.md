# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas.
   
2.Define CSV file path.

3.Read CSV into DataFrame, specifying detected encoding.

4.Display first few DataFrame rows and information.

5.Check for missing values in the DataFrame.

6.Split data into training and testing sets, train SVC model, predict labels, and calculate accuracy score. 

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Annie Jenifsika A
RegisterNumber:  212224230019

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
```

## Output:
data.head()

<img width="1171" height="364" alt="image" src="https://github.com/user-attachments/assets/1fc4ae1a-0f49-4954-9fbe-0dad1b7bfab3" />

data.info()

<img width="694" height="346" alt="image" src="https://github.com/user-attachments/assets/33a95805-08f2-468f-9acb-535d1c244e80" />

data.isnull().sum()

<img width="302" height="366" alt="image" src="https://github.com/user-attachments/assets/052e29fb-fdd4-4a79-b215-a658567e1f2c" />

y_pred

<img width="861" height="412" alt="image" src="https://github.com/user-attachments/assets/f20cd792-3370-4299-a5af-4273c4d1a02b" />

accuracy

<img width="668" height="144" alt="image" src="https://github.com/user-attachments/assets/dfcbcb6d-00f1-4088-b8a4-640cdbbb3c12" />





## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
