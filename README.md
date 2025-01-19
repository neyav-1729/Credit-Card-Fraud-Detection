# Credit-Card-Fraud-Detection
This project aims to detect fraudulent credit card transactions using machine learning techniques. The dataset is highly imbalanced, with frauds accounting for only 0.172% of the transactions. The project applies undersampling to balance the dataset and evaluates three machine learning models: Logistic Regression, Decision Tree, and Random Forest.

# Dataset
The dataset is sourced from Kaggle and consists of 284,807 transactions, of which 492 are fraudulent. It contains only numerical features, which are the result of a PCA transformation. The following features are included:

1. V1 to V28: Principal components obtained from PCA transformation (confidentialized data).
2. Time: The seconds elapsed between each transaction and the first transaction in the dataset.
3. Amount: The transaction amount.
4. Class: The target variable (1 for fraud, 0 for legitimate transactions).
5. Due to confidentiality reasons, the original features are not available.

# Approach
Data Preprocessing:

Undersampling was applied to balance the dataset, where the majority class (legitimate transactions) is reduced to match the size of the minority class (fraudulent transactions).
Modeling:

Three models were trained to detect fraudulent transactions:
Logistic Regression
Decision Tree
Random Forest
Evaluation:

The models were evaluated using the following metrics:
Accuracy
Precision
F1-score
Model Saving:

The trained models were saved using joblib for future use.

# Technologies Used
1. Python
2. Pandas for data manipulation
3. Scikit-learn for machine learning models and metrics
4. Joblib for saving models

# Installation

git clone https://github.com/your-username/credit-card-fraud-detection.git

pip install -r requirements.txt

# Usuage

Download the dataset from Kaggle. Place the dataset file in the project directory.

Run the Python script to train and evaluate the models:

bash
Copy
Edit
python credit_card_fraud_detection.py
After running the script, the trained models will be saved as:

1. Logistic_Regression_model.pkl
2. Decision_Tree_model.pkl
3. Random_Forest_model.pkl
Check the results for the evaluation metrics:

Accuracy
Precision
F1-score

# Result

The models were evaluated on the undersampled dataset. The comparison of the metrics (accuracy, precision, and F1-score) for each model is displayed at the end of the script.



