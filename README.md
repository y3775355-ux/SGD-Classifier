# SGD-Classifier
## AIM:
To write a program to predict the type of species of the Iris flower using the SGD Classifier.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1. Load the Iris dataset and separate it into input features (X) and target labels (y).
2. Standardize the feature values using StandardScaler for better model performance.
3. Split the dataset into training and testing sets using train_test_split.
4. Train an SGDClassifier model using the training data.
5. Predict using test data and evaluate performance using accuracy and classification report.

## Program:
```
/*
/*
Developed by: N.Gowsalya
RegisterNumber:  212225230085

from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.linear_model import SGDClassifier
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import accuracy_score, classification_report

iris = load_iris()
X = iris.data
y = iris.target

scaler = StandardScaler()
X = scaler.fit_transform(X)

X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

model = SGDClassifier(max_iter=1000, random_state=42)
model.fit(X_train, y_train)
y_pred = model.predict(X_test)

print("Accuracy:", accuracy_score(y_test, y_pred))

print("\nClassification Report:\n", classification_report(y_test, y_pred))

*/
Developed by: YAZHINI
RegisterNumber:  212225220126
*/
```

## Output:
![prediction of iris species using SGD Classifier](sam.png)

<img width="665" height="325" alt="Screenshot 2026-05-20 092958" src="https://github.com/user-attachments/assets/221aa98e-1c41-4c31-b858-cf3b48eb7e46" />

## Result:
Thus, the program to implement the prediction of the Iris species using SGD Classifier is written and verified using Python programming.
