# Customer Churn Prediction  
**Edunet Foundation:  Machine Learning Internship**

## Internship Task Description  

**TASK 3: CUSTOMER CHURN PREDICTION**  
Develop a model to predict customer churn for a subscription-based service or business. Use historical customer data, including features like usage behavior and customer demographics. Try algorithms like Logistic Regression, Random Forests, or Gradient Boosting to predict churn.

---

# Project: Predicting Customer Churn in the Banking Sector

## Problem Statement  
Customer attrition, or churn, is a significant challenge for banks, directly impacting revenue and growth. Retaining existing customers is more cost-effective than acquiring new ones. Therefore, predicting which customers are likely to leave allows banks to develop proactive strategies for retention.

This project aims to predict customer churn based on customer demographics and account-related behavior. By identifying high-risk customers, the bank can target retention efforts more effectively.

---

## Objective  
To develop a supervised classification model that can accurately predict whether a customer will churn or stay with the bank, using historical data of customer demographics, credit scores, and account-related behavior.

---

## Dataset Overview  

- **Industry**: Banking / Financial Services  
- **Source**: Kaggle  
- **Total Records**: Approximately 10,000 customers  
- **Target Variable**: `Exited` (1 = Churned, 0 = Retained)  
- **Features**:
  - `RowNumber`: Row number of the dataset
  - `CustomerId`: Unique identifier for each customer
  - `Surname`: Surname of the customer
  - `CreditScore`: Credit score of the customer
  - `Geography`: Location of the customer (e.g., country)
  - `Gender`: Gender of the customer (Male/Female)
  - `Age`: Age of the customer
  - `Tenure`: Number of years the customer has been with the bank
  - `Balance`: Average balance of the customer
  - `NumOfProducts`: Number of bank products the customer is using
  - `HasCrCard`: Whether the customer has a credit card (1 = Yes, 0 = No)
  - `IsActiveMember`: Whether the customer is an active member (1 = Yes, 0 = No)
  - `EstimatedSalary`: Estimated salary of the customer

---

## Tools and Technologies  

| Category            | Tools / Technologies                                    |
|---------------------|---------------------------------------------             |
| Programming Language| Python                                                   |
| Data Manipulation   | Pandas, NumPy                                            |
| Data Visualization  | Matplotlib, Seaborn                                      |
| Modeling Algorithms |Logistic Regression, Random Forests, or Gradient Boosting |
| Evaluation Metrics  | Accuracy, Precision, Recall, F1-Score, ROC-AUC           |
| Environment         | Jupyter Notebook / Python Scripts                        |

---

## STAR Methodology  

**Situation**  
A bank is experiencing a high level of customer churn, which negatively affects its profitability and growth. The bank needs a predictive model to identify customers at risk of leaving.

**Task**  
Analyze customer data and build a machine learning model to predict whether a customer will churn or not, based on demographic and financial features.

**Action**  
- Conducted exploratory data analysis (EDA) to identify patterns and relationships between features and the target variable.
- Preprocessed data by handling missing values, encoding categorical variables, and scaling numerical features.
- Trained multiple classification models including Logistic Regression, Random Forest, and XGBoost.
- Used performance metrics such as Accuracy, Precision, Recall, F1-Score, and ROC-AUC to evaluate model performance.
- Interpreted the results to identify key factors contributing to customer churn.

**Result**  
The churn prediction model achieved strong performance, with the most important features identified as `CreditScore`, `Age`, and `Balance`. These insights can be used to focus retention efforts on customers with the highest likelihood of leaving the bank.

---

## Project Structure  

```
Customer_Churn_Prediction/
├── dataset/                  # Raw and preprocessed datasets
├── notebook/             # Jupyter notebooks for EDA and modeling
│   └── Churn_Analysis.ipynb
        Model_Training.ipynb
├── src/
│   ├── preprocessing.py   # Data cleaning and transformation
│   ├── model.py           # Model training and evaluation
│   └── utils.py           # Utility functions and metrics
├── main.py                # Script to run the complete pipeline
├── requirements.txt       # List of dependencies
└── README.md              # Project documentation
```

---

## Key Insights  

- The dataset contains a mix of demographic and financial features that influence customer churn.
- Key features such as `CreditScore`, `Balance`, and `Age` were identified as important predictors for churn.
- The model's performance varied with different algorithms, with Random Forest and XGBoost delivering the best results.

---

## Future Enhancements  

- Implement SHAP or LIME for model interpretability, to better explain the predictions.
- Deploy the model using a web framework such as Flask or Streamlit for real-time prediction.
- Automate the model deployment and monitoring pipeline using tools like MLFlow or DVC.

--------------------------------------------
## How to Clone This Project and Set It Up as Your Own

### 1. Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/rashmiKumari03/CODSOFT.git
cd "CODSOFT/Customer_Churn_Prediction"
```

### 2. Create a New GitHub Repository

Go to [GitHub](https://github.com) and create a **new repository** (for example, `customer-churn-prediction`).

### 3. Reinitialize Git and Push to Your Own Repository

Now, you need to reinitialize the Git repository and link it to your new GitHub repository.

Run the following commands:

```bash
rm -rf .git           # Removes existing Git history
git init              # Initializes a new Git repository
git remote add origin https://github.com/yourusername/customer-churn-prediction.git
git add .             # Stages all files
git commit -m "Initial commit - Customer_Churn_Prediction" # Commits the files
git branch -M main    # Renames the default branch to main
git push -u origin main # Pushes your code to your new repository
```

### 4. Set Up the Conda Environment

Create a new conda environment with Python 3.10:

```bash
conda create -p venv_churn_prediction python=3.10 -y
```

Activate the environment:

```bash
conda activate ./venv_churn_prediction
```

### 5. Install Dependencies

Install the required packages from `requirements.txt`:

```bash
pip install -r requirements.txt
```

### 6. Run the Project

To run the project:

- **If you're using a Jupyter Notebook**:

  ```bash
  jupyter notebook
  ```

- **If you're running a Python script**:

  ```bash
  python main.py
  ```

---

