# Autism Prediction System

## Overview
This project implements a predictive system to detect autism using machine learning. It includes data preprocessing, model training, hyperparameter tuning, and a deployment-ready prediction function.

## Features
- Data preprocessing (handling missing values, encoding categorical data, feature selection)
- SMOTE for class balancing
- Model training using Decision Tree, Random Forest, and XGBoost
- Hyperparameter tuning with RandomizedSearchCV
- Best model selection and saving (`best_model.pkl`)
- Label encoders stored for future use (`encoders.pkl`)
- Python script to make real-time predictions

## Installation
Clone the repository and install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
Run the predictive system using:
```python
python autism_prediction.py
```

### Example Input:
```python
sample_input = {
    "A1_Score": 1,
    "A2_Score": 0,
    "A3_Score": 1,
    "A4_Score": 0,
    "A5_Score": 1,
    "A6_Score": 0,
    "A7_Score": 1,
    "A8_Score": 0,
    "A9_Score": 1,
    "A10_Score": 0,
    "gender": "male",
    "ethnicity": "White",
    "jaundice": "no",
    "austim": "yes",
    "contry_of_res": "United States",
    "used_app_before": "no",
    "relation": "Parent",
    "age": 25,
    "result": 8.5
}
```

### Output:
```bash
Autism Positive
```

## Model Training
To retrain the model:
```python
python train_model.py
```

## Files
- `autism_prediction.py` - Predictive system script
- `train_model.py` - Model training script
- `best_model.pkl` - Saved best model
- `encoders.pkl` - Label encoders
