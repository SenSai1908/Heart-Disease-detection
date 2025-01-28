# Heart-Disease-detection
This project uses machine learning techniques, specifically the Random Forest algorithm, to predict heart disease based on clinical and demographic features. It includes data preprocessing, hyperparameter tuning, and model evaluation.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Steps](#project-steps)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Heart disease is one of the leading causes of death worldwide. Early and accurate detection of heart conditions can significantly improve treatment outcomes. This project develops a predictive model to assist in identifying potential heart disease cases using patient data.

## Dataset
The dataset used in this project is stored in `heart.csv` and contains the following features:
- **Age**: Patient's age
- **Sex**: Gender of the patient
- **Chest Pain Type (cp)**: 4 types (0-3)
- **Resting Blood Pressure (trestbps)**
- **Cholesterol (chol)**
- **Fasting Blood Sugar (fbs)**: ≥ 120 mg/dl (1 = true, 0 = false)
- **Resting ECG Results (restecg)**: 0-2
- **Max Heart Rate (thalach)**
- **Exercise-Induced Angina (exang)**: 1 = yes, 0 = no
- **ST Depression (oldpeak)**
- **Target**: 1 = heart disease, 0 = no heart disease

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/SenSai1908/Heart-Disease-detection
   ```
2.Navigate to the project directory:
  ```bash
cd heart-disease-prediction
  ```
3.Install the required libraries:
  ```bash
pip install -r requirements.txt
  ```

## Usage

1.Place your dataset in the project directory as heart.csv.
2.Run the Python script to preprocess data, train the model, and evaluate performance
3.Results, including metrics and visualizations, will be displayed in the console or saved in the project folder.

## Project Steps

Data Preprocessing:
- Handled missing values and scaled numerical features.
- Addressed class imbalance using SMOTE.
Exploratory Data Analysis (EDA):
- Correlation heatmaps to identify feature relationships.
- Visualizations for feature distributions and target variable balance.
Model Building:
- Trained a Random Forest classifier.
- Performed hyperparameter tuning using GridSearchCV with parameters like n_estimators, max_depth, min_samples_split, and min_samples_leaf.
Evaluation:
- Used accuracy, precision, recall, F1-score, and confusion matrix to evaluate model performance.

## Results

- Best Hyperparameters: { 'n_estimators': 100, 'max_depth': 20, 'min_samples_split': 5, 'min_samples_leaf': 2 }
- Cross-Validation Accuracy: 92%
- Test Set Accuracy: 89%
- Confusion Matrix:
  ```bash
  [[40, 5],
   [3, 52]]
  ```

## Technologies Used

- **Python**: Programming language
- **Pandas & NumPy**: Data manipulation and analysis
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-learn**: Machine learning models and evaluation
- **Imbalanced-learn**: SMOTE for oversampling

## Contributing

- Contributions are welcome! Please open an issue or submit a pull request if you have suggestions or improvements.
  



