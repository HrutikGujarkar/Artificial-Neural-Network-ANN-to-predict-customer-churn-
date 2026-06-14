Churn Prediction Model
This notebook develops a churn prediction model using a neural network. The goal is to predict whether a customer will churn (exit the bank) based on various features.

Data
The dataset Churn_Modelling.csv contains customer information and a target variable indicating whether they have exited the bank.

Data Preprocessing
The data preprocessing steps include:

Encoding categorical features (Geography, Gender) using one-hot encoding.
Splitting the data into training and testing sets.
Scaling numerical features using StandardScaler.
Model
A Sequential Keras model is used for classification:

Input layer with 11 units and 'relu' activation.
Two hidden layers with 7 and 6 units respectively, both with 'relu' activation.
Output layer with 1 unit and 'sigmoid' activation for binary classification.
Compiled with 'adam' optimizer and 'binary_crossentropy' loss.
Results
The model's performance is evaluated using accuracy and a confusion matrix. The training history (accuracy and validation accuracy) is plotted to observe learning progress.

Metrics:
Accuracy Score: Overall correct predictions.
Confusion Matrix: Detailed breakdown of True Positives, True Negatives, False Positives, and False Negatives.
