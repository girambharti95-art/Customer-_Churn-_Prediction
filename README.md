#  Customer Churn Prediction Using Machine Learning

##  Project Overview

Customer Churn Prediction is a Machine Learning project that predicts whether a customer is likely to **leave a company or continue using its services**.

The project uses customer information such as tenure, contract type, monthly charges, total charges, and other service-related features. Machine Learning algorithms are trained on historical customer data to identify patterns related to customer churn.

The main goal is to help organizations identify customers who may leave so that appropriate customer-retention strategies can be planned.

---

##  Objectives

The main objectives of this project are:

* To understand customer churn data.
* To clean and preprocess the dataset.
* To perform Exploratory Data Analysis (EDA).
* To identify important factors affecting customer churn.
* To train Machine Learning classification models.
* To evaluate model performance using suitable metrics.
* To predict whether a customer is likely to churn.
* To provide a foundation for a future customer-churn prediction application.

---

##  Dataset

The dataset contains information about customers and their services.

Typical features may include:

* Customer ID
* Gender
* Senior Citizen
* Partner
* Dependents
* Tenure
* Phone Service
* Internet Service
* Online Security
* Online Backup
* Device Protection
* Tech Support
* Contract
* Paperless Billing
* Payment Method
* Monthly Charges
* Total Charges
* Churn

###  Target Variable

**Churn** is the target variable.

* `Yes` → Customer has left the company.
* `No` → Customer has continued using the service.

---

##  Technologies Used

| Technology                      | Purpose                   |
| ------------------------------- | ------------------------- |
| Python                          | Programming language      |
| Pandas                          | Data manipulation         |
| NumPy                           | Numerical operations      |
| Matplotlib                      | Data visualization        |
| Seaborn                         | Statistical visualization |
| Scikit-learn                    | Machine Learning          |
| Google Colab / Jupyter Notebook | Development environment   |

---

##  Project Workflow

The project follows these major steps:

```text
Dataset
   ↓
Data Collection
   ↓
Data Cleaning
   ↓
Data Preprocessing
   ↓
Exploratory Data Analysis
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Churn Prediction
```

---

##  Data Preprocessing

Before training the Machine Learning models, the dataset is prepared by performing operations such as:

1. Checking missing values.
2. Removing unnecessary columns.
3. Converting categorical data into numerical form.
4. Handling incorrect or empty values.
5. Separating input features and target variable.
6. Splitting the dataset into training and testing sets.
7. Scaling numerical features when required.

---

##  Exploratory Data Analysis

Exploratory Data Analysis is performed to understand the dataset and discover patterns.

Some useful visualizations include:

* Churn distribution
* Churn by contract type
* Churn by gender
* Churn by internet service
* Churn by payment method
* Tenure distribution
* Monthly charges distribution
* Correlation analysis

Example:

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.read_csv("customer_churn.csv")

sns.countplot(x="Churn", data=df)
plt.title("Customer Churn Distribution")
plt.show()
```

---

##  Machine Learning Models

The project can use classification algorithms such as:

### 1. Logistic Regression

Logistic Regression is used as a classification model to predict whether a customer will churn or not.

### 2. Decision Tree

A Decision Tree makes predictions using a series of decision rules based on customer features.

### 3. Random Forest

Random Forest combines multiple Decision Trees to improve prediction performance and reduce the effect of individual-tree errors.

---

##  Model Evaluation

The trained models can be evaluated using the following metrics:

### Accuracy

Measures the percentage of total predictions that are correct.

### Precision

Measures how many customers predicted as churn actually churned.

### Recall

Measures how many actual churned customers were correctly identified.

### F1-Score

Provides a balance between Precision and Recall.

### Confusion Matrix

Shows:

* True Positive
* True Negative
* False Positive
* False Negative

Example:

```python
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score

accuracy = accuracy_score(y_test, y_pred)
precision = precision_score(y_test, y_pred)
recall = recall_score(y_test, y_pred)
f1 = f1_score(y_test, y_pred)

print("Accuracy:", accuracy)
print("Precision:", precision)
print("Recall:", recall)
print("F1 Score:", f1)
```

> **Note:** Actual performance values should be added after running the models on the dataset. This README does not invent numerical results.

---

##  Churn Prediction

After training the Machine Learning model, new customer information can be provided to predict whether the customer is likely to churn.

Example input:

```text
Tenure: 5 months
Contract: Month-to-month
Monthly Charges: 75
Internet Service: Fiber optic
Tech Support: No
Payment Method: Electronic check
```

The model produces a prediction such as:

```text
Prediction: Customer is likely to churn
```

The prediction is based on the patterns learned from the training data.

---

##  Project Structure

A simple project structure can be:

```text
Customer-Churn-Prediction/
│
├── customer_churn.csv
├── customer_churn_prediction.ipynb
├── README.md
├── requirements.txt
│
└── images/
    ├── churn_distribution.png
    └── confusion_matrix.png
```

---

##  Requirements

Install the required Python libraries using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Or create a `requirements.txt` file:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
```

Then install them using:

```bash
pip install -r requirements.txt
```

---

##  How to Run the Project

### Step 1: Download or clone the project

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Open the project

Open the project folder in **VS Code** or **Google Colab**.

### Step 3: Add the dataset

Place the customer churn dataset inside the project folder.

### Step 4: Open the notebook

Open:

```text
customer_churn_prediction.ipynb
```

### Step 5: Run the code

Run the notebook cells in order:

```text
Data Loading
      ↓
Data Cleaning
      ↓
EDA
      ↓
Preprocessing
      ↓
Model Training
      ↓
Evaluation
      ↓
Prediction
```

---

##  Applications

Customer churn prediction can be useful for:

* 📱 Telecom companies
* 🏦 Banking and financial services
* 🛒 E-commerce companies
* 🎬 Subscription services
* 💻 SaaS companies
* 📺 Streaming platforms
* 🏨 Customer-service businesses

It can help businesses identify customers who may leave and understand factors associated with customer churn.

---

##  Future Scope

The project can be further improved by:

* Developing a web application using **Flask**.
* Creating a user-friendly prediction interface.
* Comparing additional Machine Learning algorithms.
* Using hyperparameter tuning.
* Improving feature engineering.
* Adding real-time prediction.
* Deploying the model on a cloud platform.
* Adding customer-retention recommendations.

---

##  Disclaimer

This project is developed for **educational and academic purposes**. The predictions depend on the quality of the dataset and the Machine Learning model used. The system should not be treated as a guarantee of future customer behavior.

---

## Author

**Bharti Giram**

Computer Engineering Student

---

## Project Purpose

This project demonstrates the complete Machine Learning workflow:

```text
Data → Preprocessing → EDA → Model Training → Evaluation → Prediction
```

It provides practical experience in **Python, Data Analysis, Data Visualization, and Machine Learning Classification**.
