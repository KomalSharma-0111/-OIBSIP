📊 Sales Prediction Using Machine Learning

📌 Overview

This project focuses on predicting product sales based on advertising expenditure across three different channels:

-  TV
-  Radio
-  Newspaper

The project uses Exploratory Data Analysis (EDA) and compares two regression algorithms — Linear Regression and Random Forest Regression — to determine which model performs better at predicting sales.

---

🎯 Objective

The main objectives of this project are to:

- Analyze the relationship between advertising expenditure and sales.
- Perform exploratory data analysis on the dataset.
- Identify which advertising channel has the strongest relationship with sales.
- Build a Linear Regression model as a baseline.
- Build a Random Forest Regression model.
- Evaluate and compare both models using MAE, RMSE, and R² Score.
- Analyze feature importance to determine the most influential advertising channel.

---

📂 Dataset

The project uses an Advertising dataset containing advertising expenditure and corresponding sales data.

Features

Feature| Description
"TV Ad Budget ($)"| Advertising expenditure on TV
"Radio Ad Budget ($)"| Advertising expenditure on Radio
"Newspaper Ad Budget ($)"| Advertising expenditure on Newspaper

Target Variable

"Sales ($)" — Product sales associated with the advertising expenditure.

The dataset was checked for missing values, and no missing/null values were found.

---

🔍 Exploratory Data Analysis

The following techniques were used:

- Dataset inspection using "head()", "info()", and "shape"
- Descriptive statistics using "describe()"
- Missing-value analysis
- Scatter plots
- Pairplot
- Correlation matrix
- Correlation heatmap

Key EDA Findings

- TV advertising has the strongest relationship with Sales.
- Radio advertising also shows a positive relationship with Sales.
- Newspaper advertising has a comparatively weaker relationship.
- The correlation between TV advertising and Sales is approximately 0.78.

---

🤖 Machine Learning Models

1. Linear Regression

Linear Regression was used as the baseline regression model.

The dataset was divided into:

- 80% training data
- 20% testing data

"random_state=42" was used for reproducibility.

2. Random Forest Regression

A Random Forest Regressor was also trained using:

- "n_estimators = 100"
- "random_state = 42"

The performance of both models was compared on the same test dataset.

---

📏 Evaluation Metrics

The models were evaluated using:

MAE — Mean Absolute Error

Measures the average absolute difference between actual and predicted sales.

Lower MAE is better.

RMSE — Root Mean Squared Error

Measures prediction error while giving greater weight to larger errors.

Lower RMSE is better.

R² Score

Measures how well the model explains the variation in the target variable.

Higher R² is better.

---

📊 Model Comparison

The notebook generates a comparison table containing:

Model| MAE| RMSE| R² Score
Linear Regression| Calculated in notebook| Calculated in notebook| Calculated in notebook
Random Forest| Calculated in notebook| Calculated in notebook| Calculated in notebook

According to the test results in the notebook, Random Forest Regression performs better than Linear Regression, with lower prediction errors and a higher R² score.


📈 Residual Analysis

A residual plot was created for the Random Forest model to examine the difference between actual and predicted sales.

Residuals were calculated as:

Residual = Actual Sales − Predicted Sales

This helps evaluate whether the model's prediction errors show any noticeable pattern.

---

🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

🚀 How to Run

1. Clone the repository

git clone <your-repository-url>

2. Navigate to the project directory

cd Sales-Prediction

3. Install the required libraries

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

4. Open the notebook

jupyter notebook Sales_prediction.ipynb

5. Run all cells

Make sure the "Advertising.csv" dataset is available and update the dataset path in the notebook if necessary.

---

💡 Key Takeaways

- Advertising expenditure can be used to build a sales prediction model.
- TV advertising shows the strongest relationship with sales in this dataset.
- Linear Regression provides a useful baseline.
- Random Forest provides better predictive performance on the test data in this project.
- Feature importance can help identify which variables are most useful for prediction.

---

🔮 Future Improvements

This project can be further improved by:

- Hyperparameter tuning of Random Forest.
- Trying additional regression algorithms such as Gradient Boosting, XGBoost, or Decision Tree Regression.
- Performing cross-validation.
- Creating a user interface for entering advertising budgets and obtaining sales predictions.
- Deploying the model using Streamlit or Flask.
- Saving the trained model using "joblib" or "pickle".

---

👩‍💻 Author

Komal Sharma
