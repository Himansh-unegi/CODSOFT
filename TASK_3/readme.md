# 📊 Advertising Sales Prediction Project 📊

This project demonstrates the prediction of sales based on advertising data using Ridge Regression. The steps include data loading, exploration, visualization, model training, evaluation, and performance visualization.

## 📋 Prerequisites

Ensure you have the following libraries installed:

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

You can install them using the following command:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## 📄 Project Overview

### Step 1: Import Necessary Libraries

The necessary libraries for data manipulation, visualization, and model building are imported.

### Step 2: Load and Explore the Dataset

- The advertising dataset is loaded using pandas.
- Basic exploratory data analysis (EDA) is performed to understand the dataset's structure and summary statistics.

### Step 3: Visualize Relationships Between Variables

- Scatter plots are created to visualize the relationships between advertising expenditures (TV, Radio, Newspaper) and Sales.

### Step 4: Calculate and Visualize Correlations

- A correlation matrix is calculated and visualized using a heatmap to understand the relationships between variables.

### Step 5: Prepare Data for Modeling

- Features (TV, Radio, Newspaper) and target variable (Sales) are defined.
- The features are standardized using `StandardScaler`.
- The dataset is split into training and testing sets.

### Step 6: Hyperparameter Tuning with Ridge Regression

- Ridge Regression is used for modeling.
- Hyperparameter tuning is performed using GridSearchCV to find the best alpha parameter for Ridge Regression.

### Step 7: Train the Ridge Regression Model

- The Ridge Regression model is trained with the best alpha parameter found in the previous step.

### Step 8: Model Evaluation

- The model's predictions are evaluated on the test set.
- Evaluation metrics such as Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), R-squared, and Adjusted R-squared are calculated and displayed.

### Step 9: Visualize Model Performance

- A scatter plot is created to visualize the Actual vs Predicted Sales.
- Residuals are plotted against predicted sales to visualize the distribution of errors.

### Step 10: Visualize Residuals

- A residual plot is created to further analyze the errors in the predictions.

### Step 11: Additional Metrics

- Mean Absolute Percentage Error (MAPE) is calculated and displayed as an additional evaluation metric.

## 🔍 Summary of Evaluation Metrics

```plaintext
Mean Absolute Percentage Error (MAPE): 8.1156%
Root Mean Squared Error (RMSE): 1.6262
Mean Absolute Error (MAE): 1.2278
R-squared: 0.8652
Adjusted R-squared: 0.8602
```

## 📈 Visualizations

- **Pairplot of Advertising Data**: Visualizes relationships between TV, Radio, Newspaper expenditures, and Sales.
- **Correlation Matrix**: Displays correlations between variables.
- **Actual vs Predicted Sales**: Scatter plot visualizing the model's performance.
- **Residual Plot**: Scatter plot visualizing the residuals (errors) in the predictions.
