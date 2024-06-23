# TASK1 Overview

Task 1 aims to predict the survival of passengers on the Titanic using machine learning techniques. The project involves data preprocessing, feature engineering, model training, evaluation, and prediction.

## Files

- `task1.ipynb`: Jupyter Notebook file containing the main code and analysis.
- `Titanic-Dataset.csv`: Dataset used in the analysis.

## Installation

To run the Jupyter Notebook (`task1.ipynb`), ensure you have the following libraries installed:

- pandas
- scikit-learn
- seaborn
- matplotlib

You can install these libraries using pip:

```bash
pip install pandas scikit-learn seaborn matplotlib
```

## Dataset

The dataset used in this project is the Titanic dataset, which contains various features such as passenger class, age, sex, number of siblings/spouses aboard, number of parents/children aboard, fare, and port of embarkation.

click me  [TitatnicDataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

## Instructions

To reproduce the analysis:

1. Open `task1.ipynb` in Jupyter Notebook.
2. Execute the cells sequentially to preprocess the data, train the model, evaluate performance, and make predictions.

## Results

## Project Structure

The project is structured as follows:

### **Data Preprocessing** :

* **Handle Missing Values** : Fill missing values in the 'Age' column with the median and in the 'Embarked' column with the mode.
* **Encode Categorical Variables** : Convert categorical variables ('Sex' and 'Embarked') into numerical format using one-hot encoding.
* **Drop Irrelevant Columns** : Remove unnecessary columns such as 'Name', 'Ticket', 'Cabin', and 'PassengerId' that do not contribute to the predictive model.

### **Feature Engineering** :

* **Select Relevant Features** : Choose the following features for model training:
  `Pclass`: Passenger class (1st, 2nd, 3rd)
  `Age`: Age of the passenger
  `SibSp`: Number of siblings/spouses aboard
  `Parch`: Number of parents/children aboard
  `Fare`: Passenger fare
  `Sex_male`: Binary encoding of passenger gender (male: 1, female: 0)
  `Embarked_Q`: Binary encoding for embarked port Queenstown (1 if embarked at Queenstown, 0 otherwise)
  `Embarked_S`: Binary encoding for embarked port Southampton (1 if embarked at Southampton, 0 otherwise)

### **Model Training and Evaluation** :

* **Gradient Boosting Classifier** : Train a Gradient Boosting Classifier using the selected features.
* **Evaluate Performance** : Assess the model's performance using the following metrics:
  * Accuracy Score: Measure of correct predictions out of total predictions.
  * Classification Report: Detailed report showing precision, recall, and F1-score for each class.
  * Confusion Matrix: Visualization of the model's performance in terms of true positives, true negatives, false positives, and false negatives.

### **Predictions** :

* **New Data Prediction** : Use the trained model to make survival predictions on new data.

## **Results**

The results of the analysis include:

**Model accuracy score : 80.44**

#### Example Data for Predictions

The following table shows the data used for making predictions:

| Pclass | Age | SibSp | Parch | Fare    | Sex_male | Embarked_Q | Embarked_S |
| ------ | --- | ----- | ----- | ------- | -------- | ---------- | ---------- |
| 1      | 22  | 2     | 5     | 41.25   | 1        | 0          | 0          |
| 3      | 38  | 1     | 0     | 7.2833  | 0        | 0          | 1          |
| 2      | 26  | 3     | 1     | 15.5    | 1        | 1          | 0          |
| 1      | 35  | 0     | 2     | 30.0    | 0        | 0          | 1          |
| 3      | 19  | 2     | 0     | 8.05    | 1        | 0          | 1          |
| 2      | 28  | 1     | 3     | 21.6792 | 0        | 1          | 0          |
| 1      | 31  | 0     | 4     | 27.0    | 1        | 0          | 0          |
| 3      | 40  | 3     | 2     | 13.0    | 0        | 0          | 1          |
| 2      | 33  | 2     | 1     | 10.5    | 1        | 1          | 0          |
| 1      | 24  | 1     | 0     | 50.0    | 0        | 0          | 1          |
| 3      | 42  | 3     | 3     | 12.475  | 1        | 0          | 0          |
| 2      | 29  | 2     | 2     | 9.0     | 0        | 1          | 1          |

Passenger 1: Did not survive
Passenger 2: Survived
Passenger 3: Did not survive
Passenger 4: Survived
Passenger 5: Did not survive
Passenger 6: Survived
Passenger 7: Did not survive
Passenger 8: Survived
Passenger 9: Did not survive
Passenger 10: Survived
Passenger 11: Did not survive
Passenger 12: Survived

## Author

- Author: Himanshu Negi
- Contact: studyhimanshustudy@gmail.com

---
