# Credit Card Fraud Detection using Machine Learning

## Project Overview

This project focuses on detecting fraudulent credit card transactions using supervised machine learning techniques. Since fraud cases represent only a very small portion of the dataset, special handling for class imbalance was required.

The project demonstrates data exploration, class imbalance handling using SMOTE, model training, performance evaluation, and visualization of results.

---

## Dataset

The dataset contains credit card transactions made by European cardholders.

### Features

* **Time**: Seconds elapsed between the transaction and the first transaction in the dataset.
* **V1 – V28**: Anonymized features obtained through PCA transformation.
* **Amount**: Transaction amount.
* **Class**:

  * 0 = Legitimate Transaction
  * 1 = Fraudulent Transaction

Dataset Size:

* Rows: 284,807
* Columns: 31

---

## Project Workflow

1. Data Loading
2. Exploratory Data Analysis (EDA)
3. Class Distribution Analysis
4. Train-Test Split
5. Handling Class Imbalance using SMOTE
6. Logistic Regression Model
7. Random Forest Model
8. Model Evaluation
9. ROC Curve Analysis
10. Feature Importance Analysis
11. Final Conclusion

---

## Technologies Used

* Python
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* Imbalanced-Learn (SMOTE)

---

## Models Implemented

### Logistic Regression

Used as a baseline classification model.

### Random Forest Classifier

Used to improve fraud detection performance and reduce false positives.

---

## Evaluation Metrics

The models were evaluated using:

* Precision
* Recall
* F1-Score
* ROC-AUC Score

Accuracy was not considered the primary metric because the dataset is highly imbalanced.

---

## Results

| Metric    | Logistic Regression | Random Forest |
| --------- | ------------------- | ------------- |
| Precision | 0.125               | 0.827         |
| Recall    | 0.898               | 0.827         |
| ROC-AUC   | 0.975               | 0.964         |

### Best Model

Random Forest was selected as the preferred model because it achieved a better balance between Precision and Recall while maintaining strong overall performance.

---

## Key Learnings

* Handling imbalanced datasets using SMOTE.
* Building supervised learning classification models.
* Evaluating models using Precision, Recall, and ROC-AUC.
* Understanding the trade-off between fraud detection and false positives.
* Visualizing model performance using Confusion Matrices and ROC Curves.

---

## Author

Harsh Gupta

Data Science Internship Project – DecodeLabs
