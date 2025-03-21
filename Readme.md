# Fraud Detection using XGBoost

## Overview
This project implements a fraud detection model using **XGBoost**, a powerful gradient boosting algorithm. The model is trained on a dataset containing transaction details and identifies fraudulent transactions.

## Features
- **Data Preprocessing**: Handles missing values, extracts features from timestamps, and encodes categorical data.
- **Model Training**: Uses XGBoost with **scale_pos_weight** to handle class imbalance.
- **Evaluation**: Provides classification metrics and ROC-AUC score.

## Installation
To set up the project, install the required dependencies:

```sh
pip install pandas scikit-learn xgboost
```

## Usage
1. Place your dataset (`transactions_train.csv`) in the project directory.
2. Run the script:

```sh
python main.py
```

3. The script will:
   - Load and preprocess data
   - Train an XGBoost model
   - Evaluate performance with a classification report and ROC-AUC score

## File Structure
```
/
│── fraud_detection.py   # Main script
│── transactions_train.csv  # Dataset (to be provided by the user)
│── README.md          # Project documentation
```

## Model Evaluation
The model is evaluated using:
- **Precision, Recall, F1-score** (from `classification_report`)
- **ROC-AUC Score** (to measure model performance on imbalanced data)

## Future Improvements
- Hyperparameter tuning for better accuracy.
- Implementing **SMOTE** or **Anomaly Detection** for handling severe imbalance.
- Deploying the model using Flask or FastAPI for real-time fraud detection.

