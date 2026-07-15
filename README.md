# Heart Disease Prediction System
A comprehensive Machine Learning project designed to predict the risk of heart disease in patients. This project explores, processes, and models medical data to achieve accurate diagnostic predictions.

## 📂 Project Overview
This project aims to leverage machine learning techniques to assist in early heart disease detection. We implemented and compared four major classification algorithms to determine which model provides the highest predictive performance.

## 🛠 Tech Stack
- **Language**: Python
- **Environment**: Google Colab
- **Libraries**: `pandas`, `numpy`, `scikit-learn`, `matplotlib`
- **Models**: 
  - Logistic Regression
  - Random Forest (with Hyperparameter Tuning)
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)

## 🚀 How to Run
1. **Open in Colab**: Click the button below to open the notebook directly in Google Colab.
   https://colab.research.google.com/drive/1elLNvBWcrDdH6N3jHbz3CmP8mQeB5zeD?usp=sharing#scrollTo=hR9DJS16ij51

2. **Upload Dataset**: 
   - Download the `heart.csv` file.
   - On the left sidebar of the Colab notebook, click the **Files** icon.
   - Upload `heart.csv` to the session.
3. **Execution**: Run all cells in the notebook sequentially.

## 📊 Methodology
- **Data Preprocessing**: Standardized numerical features using `StandardScaler` to optimize model performance.
- **Data Splitting**: Used `StratifiedShuffleSplit` to ensure proportional representation of patients and healthy individuals in both training and testing sets.
- **Optimization**: Performed `GridSearchCV` on the Random Forest model to identify the most effective hyperparameters.
- **Evaluation**: Assessed performance using:
  - **Accuracy**: Overall model performance.
  - **Recall**: Critical for medical diagnosis to minimize false negatives.
  - **ROC-AUC**: Evaluates the model's ability to distinguish between classes.

## 📈 Performance Summary
     Model              Accuracy    Precision          Recall
Logistic Regression  |  0.836066  |   0.848485    |    0.848485
Random Forest        |  0.803279  |   0.838710    |    0.787879  
KNN                  |  0.770492  |   0.787879    |    0.787879        
