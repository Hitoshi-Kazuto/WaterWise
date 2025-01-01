# WaterWise - Groundwater Vulnerability Prediction Using DRASTIC Index and Machine Learning

## Project Overview

This project predicts groundwater contamination levels using the DRASTIC index and machine learning models such as Random Forest, SVM, Logistic Regression, and XGBoost. The DRASTIC index is a widely used method for evaluating groundwater vulnerability, based on seven parameters: depth to water, net recharge, aquifer media, soil media, topography, vadose zone, and hydraulic conductivity. The project uses synthetic data to model contamination categories ('low', 'medium', 'high') and applies machine learning for classification and prediction.

## Features

### Synthetic Data Generation:

Generate synthetic DRASTIC parameters and contamination levels.
Categorize contamination levels into 'low', 'medium', and 'high'.
Machine Learning Models:

- Random Forest
- Support Vector Machines (SVM)
- Logistic Regression
- XGBoost

### Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- Mean Squared Error (MSE)
- R-Squared

### Feature Importance Analysis:

Visualize the importance of DRASTIC parameters in predicting groundwater contamination.

## Technologies Used

- **Python**: Core programming language for implementation.
- **Libraries**: pandas, numpy: Data manipulation and analysis.
- **scikit-learn**: Machine learning model training and evaluation.
- **xgboost**: Advanced gradient boosting algorithm.
- **matplotlib**: Data visualization.
- **joblib**: Model serialization.

## Setup and Installation
1. **Clone the Repository**:
```bash
git clone https://github.com/your-username/groundwater-vulnerability.git
cd groundwater-vulnerability
```

2. **Install Dependencies**:
```
pip install -r requirements.txt
```

3. **Run the Scripts:**:
```
python scripts/generate_synthetic_data.py
python scripts/train_models.py
python scripts/train_xgboost.py
python scripts/evaluate_models.py
```

## Dataset
The dataset used in this project, drastic_synthetic_data_with_contamination.csv, was synthetically generated using the DRASTIC index methodology. The dataset includes the following features:
- **Depth_to_Water**: Depth to the water table (meters).
- **Net_Recharge**: Net recharge (mm/year).
- **Aquifer_Media**: Type of aquifer material (e.g., gravel, sandstone).
- **Soil_Media**: Soil type (e.g., sandy, clayey).
- **Topography**: Land slope (%).
- **Vadose_Zone**: Zone between the surface and the water table.
- **Hydraulic_Conductivity**: Water flow capacity (m/s).
- **Land_Use**: Urban, Agricultural, or Forested.

## Results
- **Key Findings**:
   - XGBoost outperformed other models in terms of accuracy and F1-score.
   - Feature importance analysis highlighted the significant role of Depth_to_Water and Hydraulic_Conductivity.

- **Visualizations**:
   - Classification reports and accuracy comparisons are displayed in bar charts.
   - Feature importance for each model is plotted for analysis.
