# SGD-Classifier
## AIM:
To write a program to predict the type of species of the Iris flower using the SGD Classifier.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```
1.Import Necessary Libraries and Load Data 
2.Split Dataset into Training and Testing Sets
3.Train the Model Using Stochastic Gradient Descent (SGD)
4.Make Predictions and Evaluate Accuracy
```
## Program:

## Program to implement the prediction of iris species using SGD Classifier.
## Developed by: DHARAN ADITYA
## RegisterNumber: 212223040035
*/
```
import pandas as pd
from sklearn.datasets import load_iris
from sklearn.linear_model import SGDClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score, confusion_matrics
import matplotlib.pyplot as plt
import seaborn as sns
X = df.drop('target', axis=1)
y = df['target']
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
sgd_clf = SGDClassifier(max_iter=1000, tol=1e-3)
sgd_clf.fit(X_train,y_train)
y_pred = sgd_clf.predict(X_test)
accuracy = accuracy_score(y_test, y_pred)
print(f"Accuracy: {accuracy:.3f}")
cm = confusion_matrix(y_test, y_pred)
print("Confusion Matrix:")
print(cm)
```


## Output:

![368835349-817e65d2-27c8-4758-b3cf-052b473b8f3a](https://github.com/user-attachments/assets/c59ed1b0-029a-410c-882f-6bad82afbcdb)

![368835394-7fea0925-030c-4aa2-b1c8-e51c639c0f83](https://github.com/user-attachments/assets/e52cdf8f-c399-4ba5-bfab-e0ff05748d4d)

![368835423-7c0f9a5d-ec52-4ff9-84a5-e1095c3cc0c5](https://github.com/user-attachments/assets/5ab7ade7-aa93-44ba-80d9-a3a55d15fc92)

## Result:
Thus, the program to implement the prediction of the Iris species using SGD Classifier is written and verified using Python programming.
