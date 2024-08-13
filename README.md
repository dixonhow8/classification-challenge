# Module 13: Spam Email Classification Challenge

## Background

In this project, I was working on improving an email filtering system for an Internet Service Provider (ISP). The dataset provided contains information about emails classified as either spam or not spam. My task was to develop and evaluate two supervised machine learning (ML) models to accurately detect spam emails, which will help filter them out of customers' inboxes.

The models you will develop are:
1. **Logistic Regression Model**
2. **Random Forest Model**

You will compare the performance of these models to determine which is more effective at spam detection.


## Instructions

This challenge is divided into several key subsections:

### 1. Split the Data into Training and Testing Sets

1. **Read the Data:**
   - Load the data from [spam-data.csv](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv) into a Pandas DataFrame.

2. **Make Predictions:**
   - In a markdown cell, make a prediction about which model (logistic regression or random forest) you expect to perform better.

3. **Prepare the Data:**
   - Create the target variable (y) from the "spam" column.
   - Create the features DataFrame (X) from the remaining columns.

   **Note:** In the "spam" column, a value of 0 indicates a legitimate message, and a value of 1 indicates spam.

4. **Check Data Balance:**
   - Use the `value_counts` function to check the balance of the labels variable (y).

5. **Split the Data:**
   - Use `train_test_split` to divide the data into training and testing sets.

### 2. Scale the Features

1. **Create and Fit StandardScaler:**
   - Create an instance of `StandardScaler`.
   - Fit the scaler using the training data.

2. **Transform the Data:**
   - Scale both the training and testing feature DataFrames using the `transform` function.

### 3. Create a Logistic Regression Model

1. **Train the Model:**
   - Fit a logistic regression model using the scaled training data (X_train_scaled and y_train). Set the `random_state` argument to 1.

2. **Make Predictions:**
   - Save the predictions for the testing data labels using the scaled test features (X_test_scaled) and the fitted model.

3. **Evaluate the Model:**
   - Calculate and report the accuracy score of the logistic regression model.

### 4. Create a Random Forest Model

1. **Train the Model:**
   - Fit a random forest classifier model using the scaled training data (X_train_scaled and y_train).

2. **Make Predictions:**
   - Save the predictions for the testing data labels using the scaled test features (X_test_scaled) and the fitted model.

3. **Evaluate the Model:**
   - Calculate and report the accuracy score of the random forest model.

### 5. Evaluate the Models

1. **Compare Performance:**
   - In a markdown cell, answer the following questions:
     - Which model performed better?
     - How does that compare to your initial prediction?

## Author

- Howard P. Dixon
