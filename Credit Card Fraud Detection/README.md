# Credit Card Fraud Detection using Logistic Regression

This project implements a Machine Learning model to detect fraudulent credit card transactions. The dataset is highly imbalanced, so **Under-Sampling** is used to create a balanced dataset for training the model.

## 📌 Project Overview
The objective of this project is to classify transactions into two categories:
- **0**: Legitimate (Normal) Transaction
- **1**: Fraudulent Transaction

## 📊 Dataset Description
The model uses the [Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud).
- **Total Rows**: 284,807
- **Total Columns**: 31 (Time, V1-V28, Amount, Class)
- **Class Distribution**: 
  - Legitimate: 284,315
  - Fraudulent: 492

## 🛠️ Data Preprocessing & Sampling
Because the data is extremely skewed, we perform **Under-Sampling**:
1. Separate legitimate and fraudulent transactions.
2. Take a random sample of **492** legitimate transactions to match the number of fraudulent ones.
3. Concatenate these into a new, balanced dataset (984 total entries).



## 🚀 Model Training
- **Model**: Logistic Regression
- **Library**: Scikit-learn
- **Train-Test Split**: 80% Training, 20% Testing
- **Stratification**: Used to maintain the proportion of classes in both sets.

## 📈 Performance Results
The model demonstrates high reliability with the following accuracy scores:

| Dataset | Accuracy |
| :--- | :--- |
| **Training Data** | 94.66% |
| **Test Data** | 94.92% |

> **Note**: Accuracy was calculated using the `accuracy_score` metric from `sklearn.metrics`.

## 📂 Requirements
To run this project, you need the following libraries:
- `numpy`
- `pandas`
- `scikit-learn`

## 📖 Usage
1. Upload the `creditcard.csv` file.
2. Run the Jupyter Notebook or Python script.
3. The script will clean the data, balance it, and train the Logistic Regression model.

---
Created by [Your Name/Username]
