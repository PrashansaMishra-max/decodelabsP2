# 🛡️ Fraud Detection using Machine Learning

<p align="center">

![Python](https://img.shields.io/badge/Python-3.13-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-blue?style=for-the-badge&logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge&logo=scikitlearn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

</p>


# 📌 Project Overview

Fraudulent transactions pose a significant challenge in modern e-commerce, leading to financial losses and reduced customer trust. This project presents an end-to-end Machine Learning pipeline that analyzes transaction patterns and predicts potentially fraudulent orders using feature engineering, exploratory data analysis, and supervised learning models.

The project demonstrates the complete workflow of a real-world ML solution—from raw data preprocessing to business insights.


# 🎯 Problem Statement

Develop a Machine Learning model capable of identifying potentially fraudulent e-commerce transactions by analyzing customer purchase behavior and transaction characteristics.


# 📂 Dataset Information

The dataset contains **1,200 e-commerce transactions** with the following information:

- Order ID
- Customer ID
- Product Details
- Quantity
- Unit Price
- Payment Method
- Shipping Address
- Order Status
- Coupon Usage
- Referral Source
- Total Price
- Cart Information

### 📊 Engineered Features

- CouponUsed
- OrderValueCategory
- AveragePricePerItem
- CartEfficiency
- Year
- Month
- Day
- Weekday
- FraudRisk (Target Variable)


# 🧹 Data Preprocessing

The following preprocessing steps were performed:

- ✅ Removed duplicate records
- ✅ Checked missing values
- ✅ Converted Date column into datetime format
- ✅ Extracted Year, Month, Day and Weekday
- ✅ One-Hot Encoding of categorical variables
- ✅ Feature Scaling (where required)
- ✅ Train-Test Split
- ✅ SMOTE for handling class imbalance


# 📊 Exploratory Data Analysis

Several visualizations were created to understand customer purchasing behavior and identify possible fraud patterns.

| Fraud Risk Distribution | Correlation Heatmap |
|:-----------------------:|:-------------------:|
| <img src="images/fraud_distribution.png" width="450"> | <img src="images/correlation_heatmap.png" width="450"> |

| Order Status Distribution | Payment Method Analysis |
|:-------------------------:|:-----------------------:|
| <img src="images/order_status.png" width="450"> | <img src="images/payment_method.png" width="450"> |


# ⚙️ Feature Engineering

The following features were engineered to improve predictive performance:

- CouponUsed
- OrderValueCategory
- AveragePricePerItem
- CartEfficiency
- Year
- Month
- Day
- Weekday

These features capture purchasing behavior and transaction characteristics that can help distinguish potentially risky orders.


# 🤖 Machine Learning Workflow

```text
Dataset
    │
    ▼
Data Cleaning
    │
    ▼
Feature Engineering
    │
    ▼
Exploratory Data Analysis
    │
    ▼
Encoding
    │
    ▼
Train-Test Split
    │
    ▼
SMOTE
    │
    ▼
Model Training
    │
    ▼
Hyperparameter Tuning
    │
    ▼
Model Evaluation
    │
    ▼
Business Insights
```


# 🧠 Machine Learning Models

The following supervised learning models were implemented:

### 📌 Logistic Regression

- Baseline classification model
- Fast and interpretable
- Suitable for linear decision boundaries

### 🌳 Random Forest Classifier

- Ensemble learning algorithm
- Captures complex non-linear relationships
- Provides feature importance
- Hyperparameter tuning performed using GridSearchCV


# 📈 Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix

## 📊 Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|----------|-----------|--------|----------|
| Logistic Regression | 59.17% | 53.33% | 8.08% | 14.04% |
| Random Forest | 50.83% | 28.89% | 13.13% | 18.06% |
| Random Forest (GridSearchCV) | *Add Final Tuned Result* | *-* | *-* | *-* |

# 📉 Model Visualizations

### Confusion Matrix

<p align="center">
<img src="images/confusion_matrix.png" width="650">
</p>

### Feature Importance

<p align="center">
<img src="images/feature_importance.png" width="650">
</p>

### ROC Curve

<p align="center">
<img src="images/roc_curve.png" width="650">
</p>


# 💼 Business Insights

- High-value orders may require additional verification.
- Unusual cart behavior can indicate suspicious transactions.
- Coupon usage patterns provide useful indicators for fraud analysis.
- Customer purchasing behavior can improve fraud prediction.
- Feature engineering significantly enhances model performance.
- Machine Learning can support businesses in prioritizing high-risk transactions for manual review.

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Imbalanced-Learn (SMOTE)
- Jupyter Notebook


# 📁 Project Structure

```text
decodelabP2/
│
├── cleaned_dataset/
│   └── cleaned_dataset.xlsx
│
├── notebook/
│   └── fraud-detection.ipynb
│
├── images/
│   ├── fraud_distribution.png
│   ├── correlation_heatmap.png
│   ├── order_status.png
│   ├── payment_method.png
│   ├── confusion_matrix.png
│   ├── feature_importance.png
│   └── roc_curve.png
│
├── model_comparison.csv
├── README.md
├── requirements.txt
└── .gitignore
```


# 🚀 Installation & Usage

### Clone the Repository

```bash
git clone https://github.com/PrashansaMishra-max/decodelabsP2.git
```

### Navigate to the Project

```bash
cd decodelabsP2
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook inside the `notebook` folder and run all cells.


# 🚀 Future Improvements

- Train advanced models such as XGBoost and LightGBM
- Deploy the solution using Streamlit
- Build a real-time fraud detection API
- Incorporate anomaly detection techniques
- Automate model retraining with new transaction data


# 👩‍💻 Author

## **Prashansa Mishra**

🎓 B.Tech CSE (2027)

💻 Full Stack Developer | Machine Learning | Data Science Enthusiast

### Connect with Me

- **GitHub:** https://github.com/PrashansaMishra-max
- **LinkedIn:** https://www.linkedin.com/in/prashansa-mishra-50209a322/


## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

Your support motivates me to build more real-world Machine Learning and AI projects.