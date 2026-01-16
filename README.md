# credit-card-fraud-detection

End-to-end exploratory data analysis and machine learning–based detection of fraudulent credit card transactions using Python on a highly imbalanced real-world dataset.

## Problem Statement
Credit card fraud leads to significant financial losses and operational risk.  
The objective of this project is to analyze transaction behavior and build a machine learning model capable of accurately identifying fraudulent transactions while handling extreme class imbalance.

## Dataset Overview
- Dataset contains credit card transactions made by European cardholders in September 2013.
- Total transactions: 284,807
- Fraudulent transactions: 492 (0.17%)
- The dataset is highly imbalanced.
- Features V1–V28 are PCA-transformed numerical features to protect confidentiality.
- `Time` represents seconds elapsed since the first transaction.
- `Amount` represents the transaction value.
- `Class` is the target variable (1 = Fraud, 0 = Legitimate).

## Workflow

### 1. Data Understanding
- Loaded the dataset and examined structure, data types, and shape.
- Identified the target variable and confirmed severe class imbalance.
- Verified absence of missing values.

### 2. Exploratory Data Analysis (EDA)
- Analyzed class distribution to understand imbalance severity.
- Explored transaction amount patterns for fraudulent vs legitimate transactions.
- Examined time-based transaction behavior.
- Visualized feature distributions to understand data spread and variability.

### 3. Data Preprocessing
- Separated features and target variable.
- Scaled numerical features to ensure model stability.
- Prepared data for machine learning by maintaining class distribution during train-test split.

### 4. Handling Class Imbalance
- Recognized that accuracy is not a reliable metric due to imbalance.
- Focused on precision, recall, F1-score, and ROC-AUC for evaluation.
- Ensured the model prioritizes detecting fraud while minimizing false negatives.

### 5. Model Building
- Trained classification models suitable for binary fraud detection.
- Used supervised learning techniques to learn transaction patterns.
- Tuned model parameters to improve fraud detection performance.

### 6. Model Evaluation
- Evaluated model performance using:
  - Precision
  - Recall
  - F1-score
  - ROC-AUC
- Analyzed confusion matrix to understand false positives and false negatives.
- Compared results to ensure balanced performance across metrics.

### 7. Results and Insights
- Accuracy alone was avoided due to misleading results on imbalanced data.
- Precision-recall–based metrics provided meaningful evaluation.
- The model demonstrated the ability to detect fraudulent transactions effectively.

## Tools and Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Key Learnings
- Practical challenges of working with highly imbalanced datasets.
- Importance of selecting appropriate evaluation metrics.
- Real-world application of machine learning in financial fraud detection.
- Translating business problems into data-driven solutions.

## Conclusion
This project demonstrates an industry-aligned approach to fraud detection by combining exploratory data analysis, careful preprocessing, and appropriate machine learning evaluation techniques. It reflects real-world data science workflows used in financial risk and security domains.
