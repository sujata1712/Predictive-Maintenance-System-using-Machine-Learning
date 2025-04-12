# Predictive Maintenance System using Machine Learning

## Project Overview: -
This project demonstrates the development of a predictive maintenance system utilizing machine learning techniques. The model predicts potential machine failures based on sensor data, aiming to reduce unplanned downtime, enhance equipment effectiveness, and optimize maintenance schedules. The system uses the **AI4I 2020 dataset** for training and evaluation.

## Dataset: -
- **Source**: [AI4I 2020 Predictive Maintenance Dataset](https://www.kaggle.com/datasets)
- **Samples**: 10,000 records
- **Features**:
  - **Machine Type**: L (Low), M (Medium), H (High)
  - **Air Temperature**: Measured in Celsius
  - **Process Temperature**: Measured in Celsius
  - **Rotational Speed**: Machine rotational speed (RPM)
  - **Torque**: Machine torque
  - **Tool Wear**: Wear of the machine tool
- **Target**: **Machine Failure** (0 = No, 1 = Yes)

## Objective: -
The goal of this project is to:
- Predict machine failures in advance
- Reduce unplanned downtime
- Improve equipment effectiveness
- Optimize maintenance schedules

## Technologies Used: -
- **Python**
  - Libraries: `Pandas`, `NumPy`, `Seaborn`, `Matplotlib`
  - Machine Learning: `Scikit-learn`, `XGBoost`, `LightGBM`
  - Data Preprocessing: `Imbalanced-learn` (SMOTE for target balancing)
  - Model Persistence: `Joblib` (to save and load models)
- **Google Colab / Jupyter Notebook**

## Approach & Methodology: -

### Data Preprocessing
- Handled missing values (if any)
- Standardized features using **StandardScaler**
- Balanced the target variable using **SMOTE** (Synthetic Minority Over-sampling Technique)

### Model Training
Multiple machine learning models were trained and evaluated:
- **Random Forest**
- **Support Vector Machine (SVM)**
- **XGBoost**
- **LightGBM**

### Model Evaluation
Model performance was evaluated using key classification metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

### Model Selection
The **Random Forest** classifier outperformed others, achieving:
- **Accuracy**: 99.90%
- **F1-Score**: 0.9833

The best model was saved using **Joblib** for future use.

## Results: -

| Model              | Accuracy | F1 Score |
|--------------------|----------|----------|
| **Random Forest**   | 99.90%   | 0.9833   |
| **SVM**             | 98.58%   | 0.9856   |
| **XGBoost**         | 99.59%   | 0.9958   |
| **LightGBM**        | 99.48%   | 0.9948   |

## How to Run the Project: -

1. Clone the repository:
   ```bash
   git clone https://github.com/sujata1712/Predictive Maintenance System using Machine Learning.git

2. Navigate to the project directory:
   ```bash
   cd Predictive Maintenance System using Machine Learning

3. Install the required dependencies:
    ```bash  
    pip install -r requirements.txt
    
4. Open and run the Predictive-Maintenance-System.ipynb notebook in Google Colab or Jupyter Notebook.

## Conclusion: -
This project provides a comprehensive solution for predicting machine failures in industrial settings. By leveraging machine learning algorithms, the system optimizes maintenance schedules, reduces downtime, and enhances overall productivity. The approach outlined here can be applied to various industries to improve the efficiency of maintenance operations.
