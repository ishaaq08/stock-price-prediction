# About the Project

- This project involved utilising the Linear Regression model in scikit to predict the closing price of the Tesla stock based on the opening, low and high price for the day.
- The performance of the model was then evaluated by calculating the mean absolute error, mean squared error and root mean squared error.
- The dataset used was provided by [Kaggle](https://www.kaggle.com/datasets/timoboz/tesla-stock-data-from-2010-to-2020).

  # Methodology

  ### Obtaining and Preparing Data
  - Data was downloaded as CSV file and read into a DataFrame using pandas.
  - The date column was converted from an object into a datetime64 format.
  - The DataFrame was explored via pandas and matplotlib to understand the data at hand.
 
  ### Training and Testing the Data
  - Features and labels were obtained.
  - train_test_split function was used to split the data into test and training sets.
 
  ### Training the Model
  - LinearRegression class was instantiated.
  - Model was trained on training data.
 
  ### Predicting Test Data
  - Test data was passed into the model for predictions.
  - The real test values and predictions were then visualised using a scatter plot.
 
  ### Evaluating the Model and Residuals
  - To evaluate the validity of the model the mean absolute, mean squared and root mean squared errors were calculated.
  - The residuals were plotted on a distribution plot to ensure that a normal distribution was acheived.
 
  # Insights From Coefficients

- Holding all other features fixed, a 1 unit increase in the **Open** price is associated with an **decrease of 0.68 dollars in the Close price**.
- Holding all other features fixed, a 1 unit increase in the **Low** price is associated with an **increase of 0.7 dollars in the Close price**.
- Holding all other features fixed, a 1 unit increase in the **High** price is associated with an **increase of 0.9 dollars in the Close price**.

Therefore, the **High** price has the strongest relationship with the **Close** price, thus will most strongly influence it out of the 3 features (independent variables).
