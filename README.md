# 📊 Customer Retention & Churn Prediction

## 🔹 Overview  
This project builds a **churn prediction pipeline** using the [Telco Customer Churn dataset](https://www.kaggle.com/blastchar/telco-customer-churn).  
It helps businesses understand **why customers churn**, analyze **retention trends**, and predict which customers are likely to leave.  

The pipeline combines:
- **Exploratory Data Analysis (EDA)** → Visualizes churn distribution, tenure effects, and service/payment influences.
- **Feature Engineering** → Converts raw data into useful signals (tenure groups, one-hot encoding, scaled numerics).
- **Predictive Modeling** → Classification models to predict churn probability.
- **Evaluation & Visualization** → Compares models and shows churn drivers with intuitive plots.

---

## 🔹 Dataset
The dataset includes:
- **Demographics**: gender, senior citizen, partner, dependents.
- **Account info**: contract type, tenure, payment method.
- **Services**: internet, phone, streaming, security options.
- **Charges**: monthly charges, total charges.
- **Target**: `Churn` (Yes/No).

---

## 🔹 Key Steps

1. **Data Cleaning**
   - Convert string numerics (`TotalCharges`) into float.
   - Handle missing values.
   - Standardize column types.

2. **Exploratory Data Analysis**
   - Churn distribution (≈26% churn rate).
   - Churn vs tenure, contract type, payment method.
   - Monthly charges distributions.
   - Correlation heatmaps.
   - Retention survival curves with Kaplan-Meier.

3. **Feature Engineering**
   - Tenure grouping.
   - Encoding categorical variables (binary map + one-hot).
   - Scaling numeric features.

4. **Modeling**
   - Gradient Boosting
   - LightGBM

5. **Evaluation**
   - Accuracy, Precision, Recall, F1, ROC-AUC.
   - Confusion matrix.
   - Model comparison barplot.

---

## 🔹 Visuals
- 📊 **Churn distribution**  
- 📈 **Tenure vs churn rate**  
- 📉 **Monthly charges distributions**  
- 🔥 **Correlation heatmap**  
- ⏳ **Retention survival curve**  

---

## 🔹 Tech Stack
- **Python 3.9+**
- **Pandas / NumPy** (data wrangling)
- **Scikit-learn** (modeling & evaluation)
- **GradientBoosting, LightGBM** (advanced models)
- **Seaborn / Matplotlib** (visualization)
- **Lifelines** (survival analysis)
