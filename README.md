# 📊 Loan Prediction Dataset – Data Cleaning & EDA

## 📌 Project Overview
This project focuses on cleaning, preprocessing, and exploratory data analysis (EDA) of a loan prediction dataset using Python, Pandas, and Seaborn.  
The objective is to prepare a clean, analysis-ready dataset and extract meaningful business insights.

---

## 🗂 Dataset Description
The dataset contains loan applicant information used to analyze factors influencing loan amount and approval trends.

### Columns
- Loan_ID – Unique loan identifier  
- Gender – Applicant gender  
- Married – Marital status  
- Dependents – Number of dependents  
- Education – Graduate / Not Graduate  
- Self_Employed – Employment status  
- ApplicantIncome – Applicant income  
- CoapplicantIncome – Co-applicant income  
- LoanAmount – Loan amount  
- Loan_Amount_Term – Loan term (in months)  
- Credit_History – Credit history (0 or 1)  
- Property_Area – Urban / Semiurban / Rural  

---

## 🧹 Data Cleaning & Preprocessing
- Handled missing values using:
  - Median for numerical columns
  - Mode for categorical columns
- Converted appropriate columns to categorical dtype to improve performance
- Treated identifier columns correctly (kept as string)
- Fixed mixed-type columns (e.g., values like `3+`)
- Verified that no null values remain after cleaning

---

## 🧠 Data Types After Cleaning
After preprocessing, the dataset contains optimized and appropriate data types for efficient Pandas operations.

```text
category : Gender, Married, Education, Self_Employed, Property_Area
int64    : Dependents, ApplicantIncome, CoapplicantIncome,
           LoanAmount, Loan_Amount_Term, Credit_History
object   : Loan_ID
```
---
## 📊 Exploratory Data Analysis (EDA)
Exploratory Data Analysis (EDA) was performed using Pandas and Seaborn to identify patterns and trends.

### Analysis Performed

- Distribution of loan amounts
- Education vs LoanAmount analysis
- Impact of credit history on loan amount
- Property area vs income trends
- Outlier detection using boxplots
---
## 🛠 Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
---
## 💾 Saving Cleaned Dataset
The cleaned dataset is saved locally for future use:
```
df.to_csv('clean_loan_data.csv', index=False)
```
---
## 👤 Author

### Santosh Kumar Pradhan
B.Tech Student | Aspiring Data Scientist

- Skills: Python, Pandas, SQL, Data Analysis, Machine Learning
---
