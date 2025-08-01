# Loan Status Predictor using Machine Learning

This project predicts whether a loan will be **approved or not** based on various applicant details like income, credit history, employment status, etc. It's a binary classification task that leverages machine learning to assist financial institutions in making data-driven lending decisions.

---

## Dataset Description

- **Features:**
  - `Gender`
  - `Married`
  - `Dependents`
  - `Education`
  - `Self_Employed`
  - `ApplicantIncome`
  - `CoapplicantIncome`
  - `LoanAmount`
  - `Loan_Amount_Term`
  - `Credit_History`
  - `Property_Area`

- **Target:**
  - `Loan_Status` (Y = Approved, N = Not Approved)

---

## Workflow

1. **Data Cleaning**
   - Handling missing values
   - Dropping irrelevant columns (`Loan_ID`)
   - Converting categorical variables using `pd.get_dummies`

2. **Feature Scaling**
   - Applied selectively on numerical features (e.g., income, loan amount)

3. **Train-Test Split**
   - 80% training, 20% testing

4. **Modeling**
   - Primary model: `LogisticRegression`
   - GridSearchCV used for hyperparameter tuning

5. **Evaluation**
   - Classification Report
   - Confusion Matrix
   - Accuracy Score

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Reyad02/loan-status-predictor.git
   cd loan-status-predictor
   ```

2. Install dependencies:
   ```bash
    pip install -r requirements.txt
   ```

3. Run the Jupyter notebook:
   ```bash
    jupyter notebook app.ipynb
   ```

