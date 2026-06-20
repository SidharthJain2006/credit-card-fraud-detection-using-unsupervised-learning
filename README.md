
# Credit Card Fraud Detection Using Unsupervised Machine Learning

## Overview

Fraudulent transactions are extremely rare compared to legitimate transactions, making fraud detection a challenging machine learning problem. This project explores the use of unsupervised learning techniques to identify suspicious credit card transactions without relying heavily on labeled data.

The project compares two anomaly detection approaches:

- K-Means Clustering
- Isolation Forest

The objective is to identify potentially fraudulent transactions and evaluate which technique performs better on a highly imbalanced dataset.

---

## Dataset

The project uses the Credit Card Fraud Detection dataset containing:

- 284,807 transactions
- 31 features
- 492 fraudulent transactions
- 284,315 legitimate transactions

The dataset is highly imbalanced, making it a suitable candidate for anomaly detection techniques.

---

## Problem Statement

Traditional classification models often struggle when fraudulent transactions represent only a tiny fraction of the data.

This project investigates whether unsupervised machine learning algorithms can effectively identify anomalies that may correspond to fraudulent activity.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Workflow

### 1. Data Exploration

- Examined dataset structure
- Checked data types
- Verified missing values
- Generated statistical summaries

### 2. Data Visualization

- Fraud vs Non-Fraud transaction distribution
- Transaction amount distribution
- Transaction time distribution
- Correlation analysis

### 3. Data Preprocessing

- Feature scaling using StandardScaler
- Separation of features and target variable

### 4. Model Development

#### K-Means Clustering

- Created two clusters
- Identified the cluster containing the highest number of fraud cases
- Evaluated performance using classification metrics

#### Isolation Forest

- Applied anomaly detection using Isolation Forest
- Converted anomaly labels into fraud predictions
- Evaluated performance using classification metrics

---

## Model Evaluation

Evaluation metrics used:

- Confusion Matrix
- Precision
- Recall
- F1-Score
- Accuracy

### Results Summary

| Model | Frauds Detected |
|---------|----------------|
| K-Means | 155,337 |
| Isolation Forest | 570 |

### Key Findings

- K-Means generated a large number of false positives.
- Isolation Forest produced significantly fewer false positives.
- Isolation Forest proved to be more effective for anomaly detection in highly imbalanced transaction data.
- Unsupervised learning can be useful when fraud labels are unavailable or limited.

---

## Project Structure

```
├── creditcard.csv
├── ML_Fraud_Project.ipynb
├── README.md
└── images/
```

---

## Future Improvements

- Apply PCA for dimensionality reduction and visualization
- Experiment with DBSCAN and One-Class SVM
- Perform hyperparameter tuning
- Build a fraud risk scoring system
- Deploy the model using Streamlit or Flask

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Anomaly Detection
- Unsupervised Learning
- K-Means Clustering
- Isolation Forest
- Data Preprocessing
- Feature Scaling
- Model Evaluation
- Handling Imbalanced Datasets
- Fraud Detection Systems

---

## Author

**Sidharth Jain**

Aspiring Data Scientist passionate about Machine Learning, Data Analytics, and solving real-world business problems through data.
