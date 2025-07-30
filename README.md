# Credit-card-fraud-detection
Credit Card Fraud Detection – Imbalanced Data Handling
This project detects fraudulent credit card transactions using traditional machine learning models. The dataset is highly imbalanced, so multiple data balancing techniques are applied to improve performance.
Dataset
Dataset: Kaggle Credit Card Fraud Dataset
284,807 transactions, 492 frauds (~0.17% positive class).
Features: 28 anonymized PCA components (V1–V28), Time, and Amount.
Target:
2-class (default): Fraud vs. Legitimate
3-class (optional): Fraud + Legitimate split into low/high amount groups
Data Balancing Techniques
We test multiple approaches to address class imbalance:
No Balancing (Baseline)
Random Under-Sampling (RUS) – randomly remove majority samples
Random Over-Sampling (ROS) – duplicate minority samples
SMOTE – create synthetic minority class samples
SMOTEENN – hybrid of SMOTE and Edited Nearest Neighbors
Models Used
Logistic Regression (interpretable linear model)
Random Forest (tree-based ensemble model)
Each model is trained with each balancing method for comparison.
Project Flow
Data Cleaning:
Remove duplicates
Handle missing values
Train/Test Split: 80/20 split (stratified by class)
Standardization: Features are scaled using StandardScaler
Balancing & Training: Apply balancing methods, then train models
Evaluation:
Print classification report (Precision, Recall, F1-score)
Print confusion matrix
