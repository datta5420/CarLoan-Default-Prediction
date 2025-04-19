# 🚗 Car Loan Default Prediction

This project aims to predict whether a client will default on their vehicle loan using machine learning models. The solution was developed for a Hackathon hosted by a non-banking financial institution (NBFI), where minimizing the number of incorrect default predictions is crucial for business profitability.

---

## 📌 Problem Statement

An NBFI is facing significant challenges due to rising defaults in the vehicle loan segment. The goal is to build a classification model that accurately predicts the likelihood of default for each client based on their demographic, financial, and transactional features.

---

## 🎯 Objective

- Predict whether a customer will **default** on a vehicle loan (0 = No Default, 1 = Default).
- Evaluate models based on the **F1 Score**, a metric that balances **precision** and **recall**.

---

## 🗃️ Dataset Overview

There are two datasets provided:

- `Train_Dataset.csv`: Used to train the predictive model.
- `Test_Dataset.csv`: Used for making final predictions to be submitted.

### 👇 Submission Format

Your final prediction file should:

- Be a CSV file
- Contain **80900 entries + header row**
- Include two columns:
  - `ID`
  - `Default` (0 or 1)

> ✅ Example:
> ```
> ID,Default  
> 12345,1  
> 67890,0  
> ```

---

## 📊 Features

Some key features in the dataset include:

| Feature            | Description                                      |
|--------------------|--------------------------------------------------|
| ID                 | Unique Identifier for each record                |
| Disbursed Amount   | Loan amount given                                |
| Asset Cost         | Vehicle cost                                     |
| Employment Type    | Salaried or Self-Employed                        |
| Credit Score       | CIBIL Score / Creditworthiness                   |
| Loan to Value Ratio| Ratio of loan amount to asset cost              |
| Age                | Age of borrower                                  |
| EMI Amount         | Monthly installment amount                       |
| ...                | And many other financial and demographic fields  |

*Refer to `Data_Dictionary.csv` for a full list.*

---

## 🧠 Machine Learning Models Used

- Logistic Regression
- Random Forest
- XGBoost
- (Optional) LightGBM / CatBoost for further tuning

---

## 🔍 Project Workflow

1. **Data Understanding**
2. **Exploratory Data Analysis (EDA)**
3. **Handling Missing Values**
4. **Feature Engineering**
5. **Encoding Categorical Variables**
6. **Train-Test Split**
7. **Model Training**
8. **Model Evaluation using F1 Score**
9. **Final Prediction and CSV Generation**

---

## 🏆 Evaluation Metric

- **F1 Score**: Harmonic mean of Precision and Recall
- Focused on performance in class imbalance situations
- Read more: [F1 Score - Wikipedia](https://en.wikipedia.org/wiki/F-score)

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/car-loan-default-prediction.git
   cd car-loan-default-prediction
