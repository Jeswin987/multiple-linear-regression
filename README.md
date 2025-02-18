Car Performance Prediction

Overview

This project performs data preprocessing and linear regression modeling on a car dataset to predict a new target variable called Performance_Score. The dataset includes various numerical and categorical features related to car specifications, such as engine statistics, fuel efficiency, and dimensions.

Dataset

The dataset contains 5076 rows and 18 columns before preprocessing.

After removing 18 duplicate rows, we are left with 5058 rows.

The dataset contains 8 categorical variables and 9 numerical variables.

Data Preprocessing

Handling Duplicates: Removed duplicate rows.

Feature Engineering:

Created a new target variable Performance_Score using horsepower, torque, city mpg, and highway mpg.

Handling Missing Values:

Dropped rows with missing Performance_Score values.

Filled missing numerical values with the mean.

Filled missing categorical values with the mode.

Feature Selection:

Dropped irrelevant columns: Color, Condition, Dimensions.Width, Identification.ID, Identification.Year, Identification.Model Year.

Encoding Categorical Variables:

Used one-hot encoding for categorical variables.

Feature Scaling:

Applied StandardScaler to numerical features.

Model Training

Algorithm Used: Linear Regression

Train-Test Split: 80% training, 20% testing

Performance Metrics:

Mean Absolute Error (MAE): 1.6814

Mean Squared Error (MSE): 209.4048

Root Mean Squared Error (RMSE): 14.4708

R-squared Score (R²): 0.9942

Data Visualization

Residuals Plot: To check the distribution of residuals and model fit.

Histogram of Residuals: To examine the normality of residual errors.

Dependencies

Python

Pandas

Seaborn

scikit-learn

NumPy

Matplotlib

How to Run

Ensure you have Python and the required libraries installed.

Run the script in Jupyter Notebook or Google Colab.

Load the dataset (cars.csv) in the script.

Execute the script to preprocess data, train the model, and visualize results.

Future Improvements

Experiment with other regression models such as Ridge, Lasso, or Random Forest.

Perform hyperparameter tuning for better accuracy.

Add feature selection techniques to optimize model performance.

