#Customer Churn Prediction using Artificial Neural Network (ANN)


Project Overview

This project focuses on building a Customer Churn Prediction model using an Artificial Neural Network (ANN). The objective is to predict whether a bank customer is likely to exit (churn) based on their demographic and account-related features.

Accurate churn prediction helps financial institutions take proactive retention actions, improve customer satisfaction, and reduce revenue loss.

📁 Dataset

The dataset used is Churn_Modelling.csv, which contains customer information such as:

Credit Score
Geography
Gender
Age
Balance
Tenure
Number of Products
Credit Card status
Active Membership status
Estimated Salary
Target variable: Exited (0 = No churn, 1 = Churn)
🛠️ Data Preprocessing

To prepare the data for training the neural network, the following steps were performed:

Handling categorical variables
One-Hot Encoding applied to Geography
Label Encoding applied to Gender
Feature Scaling
Standardization using StandardScaler to normalize numerical features
Train-Test Split
Dataset split into training and testing sets for unbiased evaluation
Model Architecture (ANN)

A Sequential Neural Network (Keras/TensorFlow) was designed:

Input Layer: 11 input features
Hidden Layer 1: 7 neurons, ReLU activation
Hidden Layer 2: 6 neurons, ReLU activation
Output Layer: 1 neuron, Sigmoid activation (binary classification)
⚙️ Model Compilation
Optimizer: Adam
Loss Function: Binary Crossentropy
Metric: Accuracy
📈 Model Evaluation

The model is evaluated using:

Accuracy Score
Confusion Matrix
Training & Validation Accuracy curves
📊 Key Metrics Explained
🎯 Accuracy

Accuracy measures the proportion of correctly classified predictions (both churn and non-churn) out of all predictions.

However, in real-world churn datasets, accuracy alone may not be sufficient due to class imbalance.

 Why Accuracy is not enough?

In churn prediction, most customers usually do not churn, so a model can achieve high accuracy by simply predicting “no churn” most of the time.

Therefore, we also consider:

Precision: How many predicted churn customers actually churn
Recall: How many actual churn customers were correctly identified
F1 Score: Balance between precision and recall
Conclusion

The ANN model successfully learns patterns in customer behavior to predict churn. While accuracy provides a general performance overview, metrics like recall and F1-score are more important for business impact, as correctly identifying potential churners is the main goal.
