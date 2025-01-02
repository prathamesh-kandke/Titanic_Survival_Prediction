# Titanic Logistic Regression Analysis

This project demonstrates a logistic regression analysis using the Titanic dataset. The goal is to predict passenger survival based on various features of the dataset.

## Table of Contents
- [Installation](#installation)
- [Dataset](#dataset)
- [Features](#features)
- [Usage](#usage)
- [Results](#results)
- [Visualization](#visualization)

### Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Dataset
The dataset used is the Titanic dataset, which can be downloaded from [Kaggle](https://www.kaggle.com/c/titanic/data). Save the dataset as `Titanic-Dataset.csv` in the project directory.

### Columns
The dataset includes the following columns:
- **Survived**: Survival (0 = No, 1 = Yes)
- **Pclass**: Ticket class (1, 2, 3)
- **Sex**: Gender (male, female)
- **Age**: Age of the passenger
- **SibSp**: Number of siblings/spouses aboard
- **Parch**: Number of parents/children aboard
- **Fare**: Ticket fare
- **Embarked**: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Features
The following features were used for the model:
- `Pclass`
- `Sex`
- `Age`
- `SibSp`
- `Parch`
- `Fare`
- `Embarked`

Columns such as `PassengerId`, `Name`, `Ticket`, and `Cabin` were removed as they are not relevant for prediction.

## Usage

1. Preprocess the data by filling missing values and encoding categorical variables.
2. Build and train a logistic regression model using the cleaned dataset.
3. Evaluate the model using accuracy, confusion matrix, and classification report.

### Metrics
- **Accuracy**: Displays the accuracy of the model on the test dataset.
- **Confusion Matrix**: Shows the number of true positives, false positives, true negatives, and false negatives.
- **Classification Report**: Provides precision, recall, F1-score, and support for each class.

### Example Output
```
Accuracy: 0.80
Confusion Matrix:
[[89  12]
 [18  60]]
Classification Report:
              precision    recall  f1-score   support

           0       0.83      0.88      0.85       101
           1       0.83      0.77      0.80        78

    accuracy                           0.83       179
   macro avg       0.83      0.82      0.82       179
weighted avg       0.83      0.83      0.83       179
```

## Visualization

1. **Confusion Matrix Heatmap**:
   A heatmap representing the confusion matrix to visualize model performance.

   ![Confusion Matrix](confusion_matrix.png)

2. **Classification Report Heatmap**:
   A heatmap illustrating the precision, recall, and F1-score for each class.

   ![Classification Report](classification_report.png)



