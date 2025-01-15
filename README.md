# Diabetes Prediction using Machine Learning

## Overview
This project uses machine learning models to predict diabetes based on demographic and medical data. The dataset includes features like age, BMI, HbA1c level, and smoking history. Models like Logistic Regression, Random Forest, and SVM were trained to achieve high prediction accuracy.

## Dataset
The dataset contains the following features:
- `age`
- `hypertension`
- `heart_disease`
- `bmi`
- `HbA1c_level`
- `blood_glucose_level`
- `gender` (encoded as `gender_Male` and `gender_Other`)
- `smoking_history` (one-hot encoded: `current`, `ever`, `former`, `never`, `not current`)
- `diabetes` (target: 1 for diabetes, 0 for no diabetes)

**Source**: [Provide link to dataset or specify its origin]

## Models
Three models were trained and evaluated:
1. **Logistic Regression**: Accuracy - `0.96`
2. **Random Forest**: Accuracy - `0.97`
3. **Support Vector Machine (SVM)**: Accuracy - `0.96`

### Evaluation Metrics
The models were evaluated using:
- Accuracy
- Confusion Matrix
- AUROC Curve

## Preprocessing Steps
1. **Data Cleaning**:
   - Handled missing values.
   - One-hot encoded categorical features (`gender` and `smoking_history`).
2. **Scaling**:
   - Normalized numerical features using `MinMaxScaler`.
3. **Train-Test Split**:
   - 80% training and 20% testing data split.

## Predictions
The models were tested with custom input data. Example:
- **Input**: `{'age': 55, 'hypertension': 0, 'heart_disease': 1, 'bmi': 28.4, 'HbA1c_level': 6.5, 'blood_glucose_level': 140, 'gender_Male': 1, ...}`
- **Output**: 
  - Logistic Regression: `Diabetes`
  - Random Forest: `Diabetes`
  - SVM: `Diabetes`

## Files
- `diabetes_prediction.py`: Main script with data preprocessing, model training, and predictions.
- `models/`: Folder containing saved models (`.joblib`).
- `README.md`: This file.
- `requirements.txt`: Python libraries used in the project.

## How to Run
1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
# Diabetes-prediction
