# **Groundwater Vulnerability Prediction Using DRASTIC Index and Machine Learning**

## **Project Overview**
This project focuses on predicting groundwater contamination levels using the **DRASTIC index** and various machine learning models, including Random Forest, SVM, Logistic Regression, and XGBoost. The DRASTIC index is a standardized method for evaluating groundwater vulnerability based on parameters such as **depth to water, net recharge, aquifer media, soil media, topography, vadose zone, and hydraulic conductivity**.

---

## **Features**
- **Synthetic Data Generation**:
  - Generate synthetic DRASTIC parameters for training machine learning models.
  - Categorize contamination levels into `low`, `medium`, and `high`.

- **Machine Learning Models**:
  - Random Forest
  - Support Vector Machines (SVM)
  - Logistic Regression
  - XGBoost

- **Evaluation Metrics**:
  - Accuracy, Precision, Recall, F1-score, Mean Squared Error (MSE), and R-squared.

- **Feature Importance Analysis**:
  - Visualize the importance of different DRASTIC parameters.

---

## **Technologies Used**
- **Python**: Core programming language.
- **Libraries**:
  - `pandas`, `numpy`: Data manipulation and analysis.
  - `scikit-learn`: Machine learning model training and evaluation.
  - `xgboost`: Advanced gradient boosting algorithm.
  - `matplotlib`: Data visualization.
  - `joblib`: Model serialization.

---

## **Project Structure**
```plaintext
.
├── data/
│   └── drastic_synthetic_data_with_contamination.csv  # Synthetic dataset
├── models/
│   ├── random_forest_model.joblib                     # Trained Random Forest model
│   ├── svm_model.joblib                               # Trained SVM model
│   ├── logistic_regression_model.joblib              # Trained Logistic Regression model
│   └── xgboost_model.joblib                          # Trained XGBoost model
├── scripts/
│   ├── generate_synthetic_data.py                    # Script to generate synthetic data
│   ├── train_models.py                               # Train RF, SVM, Logistic Regression models
│   ├── train_xgboost.py                              # Train the XGBoost model
│   └── evaluate_models.py                            # Evaluate models and visualize results
├── requirements.txt                                  # List of dependencies
└── README.md                                         # Project documentation


