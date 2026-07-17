# churn-ai-ml-
# 📊 Telco Customer Churn Prediction using Machine Learning

## 📌 Project Overview

This project predicts whether a telecom customer is likely to **churn (leave the service)** using a **Random Forest Classifier**. The model is trained on the popular **Telco Customer Churn Dataset** and uses customer demographic information, account details, and service usage patterns to make predictions.

---

## 🎯 Objective

The goal of this project is to:

* Analyze customer data.
* Identify customers likely to churn.
* Build a machine learning model for churn prediction.
* Evaluate model performance using classification metrics.

---

## 📂 Dataset

**Dataset:** Telco Customer Churn Dataset

The dataset contains information such as:

* Customer demographics
* Service subscriptions
* Account information
* Monthly charges
* Total charges
* Churn status

**Target Variable:**

* `Churn`

  * 0 → Customer Stays
  * 1 → Customer Leaves

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Random Forest Classifier
* Jupyter Notebook / Google Colab

---

## 📦 Required Libraries

Install dependencies using:

```bash
pip install pandas numpy scikit-learn
```

---

## 🔄 Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas:

```python
df = pd.read_csv('WA_Fn-UseC_-Telco-Customer-Churn.csv')
```

### 2. Data Preprocessing

* Remove unnecessary columns (`customerID`)
* Convert `TotalCharges` to numeric format
* Handle missing values using median imputation
* Encode categorical features using Label Encoding

### 3. Train-Test Split

```python
train_test_split(
    X, y,
    test_size=0.2,
    random_state=42,
    stratify=y
)
```

* Training Data: 80%
* Testing Data: 20%

### 4. Model Training

Random Forest Classifier:

```python
RandomForestClassifier(
    n_estimators=200,
    random_state=42
)
```

### 5. Model Evaluation

Performance metrics:

* Accuracy Score
* Classification Report
* Confusion Matrix

### 6. Feature Importance Analysis

The model identifies the most influential features affecting customer churn.

---

## 📈 Model Evaluation Metrics

The model outputs:

```text
Accuracy Score
Classification Report
Confusion Matrix
```

Example:

```text
Accuracy: 0.80
```

*(Actual results may vary depending on preprocessing and dataset version.)*

---

## 🔍 Important Features

The model ranks features according to their contribution to churn prediction.

Common important features include:

* Contract
* MonthlyCharges
* TotalCharges
* tenure
* InternetService
* PaymentMethod

---

## 📁 Project Structure

```text
Telco-Customer-Churn/
│
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── churn_prediction.py
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/telco-customer-churn.git
```

2. Navigate to the project folder:

```bash
cd telco-customer-churn
```

3. Install dependencies:

```bash
pip install pandas numpy scikit-learn
```

4. Run the Python script:

```bash
python churn_prediction.py
```

---

## 📊 Machine Learning Algorithm

### Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

Advantages:

* High accuracy
* Handles large datasets effectively
* Provides feature importance rankings
* Robust against overfitting

---

## 🚀 Future Improvements

* Hyperparameter tuning using GridSearchCV
* Compare multiple algorithms

  * Logistic Regression
  * XGBoost
  * Gradient Boosting
  * Support Vector Machine
* Deploy the model using Flask or Streamlit
* Build an interactive dashboard

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Submit a Pull Request

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Ayyanar Kanna P**

Bachelor Computer Application Degree (UG) – 2027
Kamaraj College

Machine Learning | Data Science | Full Stack Development
