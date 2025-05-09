# House Price Prediction using Linear Regression

This project aims to predict house prices using a linear regression model based on key features like living area and total rooms (bedrooms + bathrooms). The project uses the popular 'House Prices - Advanced Regression Techniques' dataset from Kaggle.


## Project Overview

The project follows these key steps:

1. **Data Loading:** Loads the training and testing datasets from CSV files.
2. **Data Exploration:** Analyzes the distributions of key features and their relationships with the target variable ('SalePrice').
3. **Data Cleaning:** Handles missing values and outliers in the data.
4. **Feature Engineering:** Creates a new feature 'total_rooms' by combining bedroom and bathroom counts.
5. **Data Splitting:** Splits the training data into training and validation sets.
6. **Model Training:** Trains a linear regression model on the training data.
7. **Model Evaluation:** Evaluates the model's performance using metrics like Mean Squared Error (MSE), R-squared, and Root Mean Squared Error (RMSE).
8. **Prediction:** Applies the trained model to the test data to predict house prices.
9. **Submission:** Generates a submission file in the required format for Kaggle.


## Key Features and Target Variable

* **GrLivArea:** Above grade (ground) living area square feet.
* **BedroomAbvGr:** Number of bedrooms above grade.
* **FullBath:** Number of full bathrooms.
* **total_rooms:** Combined number of bedrooms and full bathrooms (engineered feature).
* **SalePrice:** The target variable representing the sale price of the house.


## Data Cleaning and Preprocessing

* **Missing Values:** Imputed using the median value of the respective feature in the training data.
* **Outliers:** Handled using the Interquartile Range (IQR) method, clipping values outside a calculated range.


## Model and Evaluation

* **Model:** Linear Regression
* **Evaluation Metrics:** MSE, R-squared, RMSE


## Results

The linear regression model achieved an R-squared value of approximately 0.588 on the validation set, indicating that it explains about 59% of the variance in house prices. The RMSE was around 44878.67.


## Insights and Next Steps

* Explore other potential features or feature combinations to improve model performance.
* Experiment with different regression models like Ridge, Lasso, or Random Forest.
* Evaluate the models using more comprehensive techniques like cross-validation.


## How to Use

1. **Download the dataset:** Get the 'House Prices - Advanced Regression Techniques' dataset from Kaggle and place the CSV files in the project directory.
2. **Run the code:** Execute the Jupyter Notebook or Python script provided to train the model, make predictions, and generate the submission file.
