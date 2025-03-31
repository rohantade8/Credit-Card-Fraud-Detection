```markdown
# Credit Card Fraud Detection

## Overview

This project implements a credit card fraud detection system using **Logistic Regression**. The model is trained on a dataset of credit card transactions to classify transactions as either legitimate or fraudulent. This helps in identifying and preventing fraudulent activities, thereby minimizing financial risks.

## Dataset

The dataset used in this project is sourced from Kaggle: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

### Dataset Information:

-   **Total Transactions:** 284,807
-   **Fraudulent Transactions:** 492
-   **Features:** 30 anonymized features (V1, V2, ..., V28), `Time`, and `Amount`.
-   **Target Variable:** `Class` (1 for fraudulent, 0 for legitimate).
-   **Data Split:** The dataset consists of 284,807 rows and 31 columns, with the `Class` column being the target variable.

## Requirements

To run this project, you need the following Python libraries:

-   Python 3.x
-   Streamlit
-   Pandas
-   Scikit-learn
-   Joblib
-   NumPy

### Installation:

```bash
pip install -r requirements.txt
```

## How to Use

1.  **Download the Dataset:** Obtain the `creditcard.csv` file from the Kaggle dataset link provided above.
2.  **Run the Streamlit App:** Execute the following command in your terminal:

    ```bash
    streamlit run app.py
    ```

3.  **Upload Data:** Upload a CSV file containing credit card transaction data through the Streamlit interface.
4.  **Get Predictions:** The model will predict and display the fraudulent transactions.
5.  **Download Results:** Download the prediction results as a CSV file.

## Project Structure

```
Credit-Card-Fraud-Detection/
├── app.py           # Streamlit application for fraud prediction
├── model.py         # Model training and saving script
├── fraud_model.pkl  # Pre-trained Logistic Regression model
├── preprocess.py    # Data preprocessing script
├── requirements.txt # Project dependencies
└── README.md        # Project documentation
```

## Model

The model used in this project is **Logistic Regression**, a binary classification algorithm.

### Why Logistic Regression?

-      Simplicity and Efficiency: It is a simple and efficient algorithm for binary classification.
-      Structured Data: It performs well on structured datasets like the one used in this project.
-      Probability Scores: It provides probability scores, which are useful for setting fraud detection thresholds.

### Model Training Steps:

1.  **Preprocessing:** Data cleaning (handling missing values) and feature scaling.
2.  **Training:** Training the Logistic Regression model on the preprocessed data.
3.  **Evaluation:** Model evaluation using cross-validation and metrics such as accuracy, precision, recall, and ROC-AUC.
4.  **Saving:** Saving the trained model using Joblib.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## Acknowledgments

-      Dataset provided by MLG ULB from Kaggle.
-      Streamlit for providing a user-friendly interface for deploying machine learning applications.

## Additional Information

-   **Model:** Logistic Regression.
-   **Application:** User-friendly Streamlit application for uploading transaction data and receiving fraud predictions.
-   **Feature Importance:** Logistic regression provides insights into feature importance through model coefficients.
-   **Deployment:** Streamlit is used for easy deployment and interaction with the model.
```
