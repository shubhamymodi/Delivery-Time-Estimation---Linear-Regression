# 🚚 Delivery Time Estimation – Linear Regression

A machine learning project that predicts **food delivery time** using historical delivery data.  
The goal is to help logistics platforms estimate accurate delivery times and improve operational efficiency.

This project demonstrates **data cleaning, feature engineering, regression modeling, and model evaluation using Python.**

---

## 📌 Problem Statement

Food delivery platforms must provide **accurate delivery time estimates** to maintain customer satisfaction and optimize logistics operations.

Delivery time depends on several factors such as:

- Delivery distance  
- Restaurant preparation time  
- Order volume  
- Operational demand  

This project builds a **regression model to estimate delivery time** based on these operational variables.

---

## 📊 Dataset

The dataset contains **140K+ delivery records** with operational attributes affecting delivery performance.

### Key Variables

- Order ID  
- Restaurant ID  
- Delivery Distance  
- Order Time  
- Preparation Time  
- Traffic / demand indicators  
- Delivery Time (Target Variable)

---

## 🧹 Data Cleaning

The dataset required several preprocessing steps:

- Removed duplicate records  
- Handled missing values  
- Converted timestamp columns into usable features  
- Detected outliers using **IQR method**  
- Applied **outlier capping** to stabilize regression performance  

These steps ensured a **clean dataset suitable for modeling**.

---

## ⚙️ Feature Engineering

Feature engineering improved model performance through:

- Distance-based features  
- Time-based features  
- Categorical encoding  
- Feature scaling

Feature selection techniques used:

- **Variance Inflation Factor (VIF)** to detect multicollinearity  
- **Recursive Feature Elimination (RFE)** to select important predictors

---

## 🤖 Model Development

The model used:

**Multiple Linear Regression**

Libraries used:

- Scikit-learn  
- Statsmodels  

The model learns relationships between delivery time and operational variables.

---

## 📈 Model Performance

| Metric | Value |
|------|------|
| RMSE | ~5 minutes |
| R² Score | 0.62 |

### Interpretation

- The model explains **62% of the variance in delivery time**
- Predictions are typically **within ~5 minutes of actual delivery time**

---

## 🔍 Key Insights

### 1️⃣ Delivery Distance
Delivery distance has a strong positive relationship with delivery time.

### 2️⃣ Order Load
Higher order volumes increase delivery delays.

### 3️⃣ Restaurant Preparation Time
Preparation time significantly contributes to delivery duration.

### 4️⃣ Demand Peaks
Peak hours lead to longer delivery times due to operational congestion.

---

## 🛠 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Statsmodels  
- Matplotlib    

---

## 📈 Business Value

Accurate delivery time prediction helps businesses:

- Improve **customer satisfaction**
- Optimize **delivery logistics**
- Reduce **late deliveries**
- Enable **better operational planning**

---
