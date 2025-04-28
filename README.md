# Credit Card Fraud Detection

## Context

It is crucial for credit card companies to detect fraudulent transactions to prevent customers from being charged for purchases they did not make.

## About the Dataset

- **Source**: Credit card transactions made by European cardholders in September 2013.
- **Period**: Data collected over two days.
- **Size**: 284,807 transactions, with 492 fraud cases (0.172%).
- **Features**:
  - Only numerical variables (PCA-transformed).
  - `V1` to `V28`: Principal components obtained with PCA.
  - `Time`: Seconds elapsed between each transaction and the first transaction.
  - `Amount`: Transaction amount.
  - `Class`: Target variable (1 = fraud, 0 = legitimate).

> **Note**: Original features and additional background information are not available due to confidentiality issues.

## Challenge

Given the severe class imbalance, it is recommended to evaluate model performance using the **Area Under the Precision-Recall Curve (AUPRC)**. Traditional accuracy metrics are misleading for imbalanced datasets.

---

## About This Project

This project implements a machine learning pipeline to detect credit card fraud, including:

- Exploratory data analysis;
- Data preprocessing and handling of class imbalance;
- Training of classification models;
- Evaluation focused on metrics suited for imbalanced data.

### Models Used

- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest

---

## Results

### K-Nearest Neighbors (KNN)

- Accuracy: **1.00**
- Balanced Accuracy: **0.90**
- Precision: **1.00**
- Recall: **1.00**
- F1 Score: **1.00**
- Average Precision (AUPRC): **0.75**

**Cross-validation Performance**:
- Mean Accuracy: **1.00**
- Cross-validation Accuracy Standard Deviation: **0.00**
- Mean Balanced Accuracy: **0.85**
- Mean F1 Score: **0.77**
- Mean Precision: **0.88**
- Mean Recall: **0.70**
- Mean Average Precision: **0.69**

---

### Decision Tree

- Accuracy: **1.00**
- Balanced Accuracy: **0.85**
- Precision: **1.00**
- Recall: **1.00**
- F1 Score: **1.00**
- Average Precision (AUPRC): **0.50**

**Cross-validation Performance**:
- Mean Accuracy: **0.90**
- Cross-validation Accuracy Standard Deviation: **0.29**
- Mean Balanced Accuracy: **0.80**
- Mean F1 Score: **0.59**
- Mean Precision: **0.60**
- Mean Recall: **0.70**
- Mean Average Precision: **0.41**

---

### Random Forest

- Accuracy: **1.00**
- Balanced Accuracy: **0.89**
- Precision: **1.00**
- Recall: **1.00**
- F1 Score: **1.00**
- Average Precision (AUPRC): **0.74**

**Cross-validation Performance**:
- Mean Accuracy: **1.00**
- Cross-validation Accuracy Standard Deviation: **0.00**
- Mean Balanced Accuracy: **0.87**
- Mean F1 Score: **0.79**
- Mean Precision: **0.90**
- Mean Recall: **0.73**
- Mean Average Precision: **0.78**

---

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---

## License

Distributed under the MIT License.  
See `LICENSE` for more information.
