# Credit Card Fraud Detection

## Overview
This project aims to predict fraudulent credit card transactions using machine learning. The model is trained on a dataset of credit card transactions and can classify transactions as either legitimate or fraudulent.

## Dataset
The dataset used in this project is from Kaggle, and it contains 284,807 transactions, with 492 of them being fraudulent. You can access the dataset [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

### Dataset Information:
- **Features**: The dataset contains 30 anonymized features, along with a target column (`Class`), which indicates whether a transaction is fraudulent (1) or not (0).
- **Data Split**: The dataset is split into **284,807 records** (rows) and **31 features** (columns), with the last column (`Class`) being the target variable.
  
## Requirements
To run the project, you need the following libraries:

- Python 3.x
- Streamlit
- Pandas
- Scikit-learn
- Joblib
- NumPy

### Install dependencies:
```bash
pip install -r requirements.txt
# Credit-Card-Fraud-Detection
