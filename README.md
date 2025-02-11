# Customer Churn Analysis & Prediction

## 📌 Project Overview
This project analyzes **customer churn** using the **Telco Customer Churn dataset** from Kaggle. The goal is to **explore churn patterns** and **build a predictive model** to identify customers likely to leave.

## 📊 Dataset Information
- **Source**: [Telco Customer Churn - Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Size**: ~7,000 customer records
- **Key Features**:
  - Customer demographics (gender, senior citizen, partner, dependents)
  - Subscription details (tenure, contract type, payment method)
  - Financial information (monthly & total charges)
  - **Target Variable**: `Churn` (Yes/No)

## 📈 Exploratory Data Analysis (EDA)
Key findings from the dataset:
- **Churn Rate**: ~26% of customers churned.
- **Higher Churn in Monthly Contracts**: Customers on month-to-month contracts churn more than those with longer commitments.
- **Payment Method Impact**: Customers paying with electronic checks have the highest churn rate.
- **Tenure & Churn**: Long-tenure customers are less likely to churn.

### 🔍 Visual Insights
- Distribution of churn customers:
  - ![Churn Distribution](images/churn_distribution.png)
- Monthly charges and total charges impact:
  - ![Monthly Charges vs Churn](images/monthly_charges_vs_churn.png)

## 🚀 Machine Learning Model
### **1. Data Preprocessing**
- Converted categorical features to numerical (One-Hot Encoding)
- Handled missing values & scaled numerical features

### **2. Model Training**
- **Algorithms Tested:**
  - Logistic Regression
  - Random Forest
  - XGBoost (Best performing)
- **Best Model Performance:**
  - **Accuracy**: ~82%
  - **Precision**: 78%
  - **Recall**: 74%

## 📌 How to Use
### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/churn-analysis.git
cd churn-analysis
```

### **2. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3. Run the Jupyter Notebook**
```bash
jupyter notebook churnproj.ipynb
```

## 📊 Deployment
- **API**: Flask-based prediction API (optional)
- **Docker**: Ready-to-use Dockerfile for containerized deployment

## 🔗 Links
- 📂 **Dataset**: [Kaggle Link](https://www.kaggle.com/blastchar/telco-customer-churn)
- 📝 **Notebook**: [Google Colab](https://colab.research.google.com/your-colab-link)
- 📜 **GitHub Repo**: [churn-analysis](https://github.com/yourusername/churn-analysis)

## 📌 Future Improvements
- Feature engineering for better predictive performance
- Deploy as a FastAPI service for real-time predictions
- Improve visualization dashboard for business insights
