# Credit Card Fraud Detection System
# Objective: 
The goal of this project is to build a machine learning model that can detect fraudulent transactions based on transaction details such as cc_num,	merchant,	category,	amt,	gender,	lat,	long,	city_pop,	merch_lat,	merch_long,	hour,	day_of_week.

# Aim of this project:
A fraud detection system that minimizes false positives while maximizing fraud detection accuracy.

# Project step:

1. Data Preprocessing
   - Handled missing values.
   - drop unrequired feature (those who not help to find the fraud) such as Unnamed: 0, first, last, street, city, state, zip, dob, trans_num, unix_time, job.
   - Feature engineering: Extracted 'hour', 'day_of_week' from transaction timestamp.
   - Label encoding for categorical features.
   - Feature scaling with StandardScaler.

2. Model Building
   - Used Random Forest Classifier for classification.
   - Balanced class weights due to data imbalance.
   - Hyperparameter tuning for better performance.

3. Model Evaluation
   - Metrics used: Accuracy,confusion_matrix, roc_auc_score.
   - Classification Report: Precision, Recall, F1-Score, support.
   - Confusion Matrix analyzed for misclassifications.

4. Explainability
   - Top Feature importance visualization.
   - High Recall value means the model caugth more fraud.
   - High Receiver Operating Characteristic(ROC) values means How many real fraudsters were caught it means your model good.
