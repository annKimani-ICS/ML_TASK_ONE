Nairobi Office Price Prediction Model
This project builds a linear regression model to predict office prices based on office size using the provided "Nairobi Office Price Ex" dataset. It includes functions to calculate Mean Squared Error (MSE) as a performance metric and uses Gradient Descent to update the model parameters. The model is trained for a set number of epochs, with error values displayed for each epoch, and a final plot shows the line of best fit.

Table of Contents
Installation
Dataset
Project Overview
Functions
Running the Model
Results
License
Installation
Clone the repository:

bash
Copy code
git clone <your-repository-link>
cd <your-repository-directory>
Install dependencies:

bash
Copy code
pip install numpy matplotlib pandas
Dataset
Dataset Name: Nairobi Office Price Ex
Features:
x: Office size (in square feet)
y: Office price
Format: Ensure your dataset is in CSV format and contains two columns (x for office size and y for office price).
Project Overview
The objective of this project is to create a linear regression model that can predict office prices based on office size. The following steps are covered:

Initialize Parameters: Randomly assign values for slope (m) and y-intercept (c).
Calculate Mean Squared Error (MSE): Use MSE as a performance measure to evaluate the accuracy of predictions.
Apply Gradient Descent: Update the weights using gradient descent.
Train the Model: Train for 10 epochs, showing the MSE after each epoch.
Plot Line of Best Fit: Plot the line of best fit after training.
Make Predictions: Use the trained model to predict office prices, e.g., for an office size of 100 sq. ft.
Functions
1. mean_squared_error(y_true, y_pred)
Calculates the Mean Squared Error (MSE) to evaluate model performance.

Input:

y_true: Array of actual prices
y_pred: Array of predicted prices
Output: MSE (float)

2. gradient_descent(x, y, m, c, learning_rate)
Performs one step of gradient descent to update slope (m) and y-intercept (c).

Input:

x: Array of office sizes
y: Array of actual prices
m: Current slope
c: Current y-intercept
learning_rate: Step size for gradient descent
Output: Updated m and c values

Running the Model
Load the Dataset: Load the dataset into a Pandas DataFrame.

Initialize Parameters: Set initial values for m (slope) and c (y-intercept) randomly.

Train the Model:

Run gradient descent for 10 epochs.
Compute and print the MSE at each epoch.
Plot Results: Plot the line of best fit after training.

Make Prediction: Predict office price for a 100 sq. ft office.
