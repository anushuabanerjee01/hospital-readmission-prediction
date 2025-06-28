# hospital-readmission-prediction

# 🏥 Hospital Readmission Prediction Using Logistic Regression & Neural Networks

## 🔍 Problem Statement
This project aims to predict whether a patient will be readmitted to the hospital within 30 days based on diagnosis, treatment history, and hospital-related variables. Additionally, we assess whether an initial diagnosis of diabetes is a significant predictor of readmission.

## 📊 Tools & Technologies
- Python (pandas, scikit-learn, matplotlib)
- Logistic Regression & Neural Networks (MLPClassifier with GridSearchCV)
- Feature selection techniques (Forward, Backward, Stepwise)
- Evaluation: Confusion Matrix, AUC, Gains Chart, Lift Chart
- Jupyter Notebook, Excel, Matplotlib

## 🧬 Dataset
- Source: [Kaggle - Hospital Readmissions](https://www.kaggle.com/datasets/dubradave/hospital-readmissions/data)
- Size: 25,000 records | 17 features (converted to 46 after one-hot encoding)
- Features include: length of stay, ICD diagnoses, lab procedures, diabetes medication, A1C tests, age, etc.

## 🔢 Key Steps
- Cleaned and preprocessed data using one-hot encoding for categorical features
- Modeled with Logistic Regression (multiple configurations)
- Used Neural Networks with hyperparameter tuning (Grid Search on hidden layer size)
- Compared models using accuracy, gains/lift charts, and confusion matrices

## 💡 Insights
- Patients with **diabetes as a primary diagnosis** are significantly more likely to be readmitted
- Logistic Regression model achieved ~61.57% accuracy
- Neural Network (best model): ~61.92% validation accuracy
- Factors like **A1C test skipped**, **medication change**, and **diabetes medication prescribed** correlated with increased readmission likelihood

## 📊 Visuals
- Gains & Lift Charts show lift of 1.6 in top decile
- Confusion matrices demonstrate consistent performance (no overfitting)

## 📁 Project Structure
