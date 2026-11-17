# Customer Churn Prediction using Artificial Neural Network (ANN)

## Project Overview

This project uses an Artificial Neural Network (ANN) to predict whether a bank customer is likely to leave the bank or continue using its services.

The model learns patterns from customer information such as age, credit score, balance, geography, gender, and account activity to classify customers into two categories:

- **0 – Not Exited:** Customer continues using the bank's services.
- **1 – Exited:** Customer has left the bank.

The project demonstrates an end-to-end machine learning workflow, including data preprocessing, feature scaling, neural network development, model training, and evaluation.

## Dataset

- **Dataset:** Churn Modelling
- **Source:** Kaggle – [Credit Card Customer Churn Prediction](https://www.kaggle.com/datasets/rjmanoj/credit-card-customer-churn-prediction)
- **Total Records:** 10,000
- **Original Features:** 14
- **Target Variable:** `Exited`

The dataset contains customer information, including:

- Credit Score
- Geography
- Gender
- Age
- Tenure
- Balance
- Number of Products
- Credit Card Status
- Active Member Status
- Estimated Salary

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- TensorFlow
- Keras
- Google Colab
- KaggleHub

## Project Workflow

1. **Data Collection:** Downloaded the dataset using KaggleHub.
2. **Data Exploration:** Examined dataset structure, statistical information, missing values, and duplicate records.
3. **Data Preprocessing:** Removed unnecessary columns such as RowNumber, CustomerId, and Surname.
4. **Categorical Encoding:** Applied One-Hot Encoding using `pd.get_dummies()`.
5. **Feature Selection:** Separated independent variables (X) and the target variable (y).
6. **Train-Test Split:** Divided the dataset into training and testing sets.
7. **Feature Scaling:** Applied StandardScaler to standardize numerical input features.
8. **ANN Model Development:** Built a neural network using TensorFlow and Keras.
9. **Model Training:** Trained the model using the Adam optimizer and Binary Crossentropy loss function.
10. **Model Evaluation:** Evaluated predictions and visualized training and validation performance.

## ANN Architecture

The Artificial Neural Network consists of:

| Layer | Neurons | Activation |
|---|---:|---|
| Input Layer | 11 | — |
| Hidden Layer 1 | 11 | ReLU |
| Hidden Layer 2 | 11 | ReLU |
| Output Layer | 1 | Sigmoid |

### Model Configuration

- **Optimizer:** Adam
- **Loss Function:** Binary Crossentropy
- **Evaluation Metric:** Accuracy
- **Training Epochs:** 100
- **Output:** Binary classification (0 or 1)

## Model Evaluation and Visualization

The project includes:

- Training and validation accuracy visualization.
- Training and validation loss visualization.
- Customer churn predictions on test data.
- Accuracy evaluation.

## How to Run the Project

The notebook is designed to run in Google Colab.

1. Open the notebook from the repository.
2. Select **Open in Colab**.
3. Install KaggleHub if it is not already available:

   ```python
   !pip install kagglehub
   ```

4. Run the notebook cells sequentially.
5. The dataset will be downloaded using KaggleHub.
6. Execute preprocessing, model training, prediction, and evaluation cells.

## Repository Structure

```text
Customer-Churn-Prediction-ANN/
│
├── Customer_Churn_Prediction_using_ANN.ipynb
└── README.md
```

## Project Objective

The main objective is to apply deep learning techniques to a customer churn prediction problem and understand how Artificial Neural Networks can identify patterns in customer data for binary classification.

## Author

**Manoj Kumar**

GitHub: [kumarm48759-code](https://github.com/kumarm48759-code)
