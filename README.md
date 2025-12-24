
```markdown
# 📊 Customer Churn Analysis & Prediction

This project performs **end-to-end customer churn analysis**, including Exploratory Data Analysis (EDA), feature engineering, machine learning model building, and deployment using a **Flask web application**.

The goal is to identify customers who are more likely to churn and provide a predictive system that can be accessed via a web UI.

---

## 🔍 Problem Statement
Customer churn is a critical challenge for subscription-based businesses. This project aims to:
- Analyze customer behavior
- Identify churn-driving factors
- Build a robust churn prediction model
- Deploy the model using a Flask API

---

## 🛠️ Tech Stack
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn, Imbalanced-learn (SMOTEENN)
- **Model:** Random Forest Classifier
- **Deployment:** Flask
- **Frontend:** HTML (Jinja Templates)

---

## 📁 Project Structure
```

Customer Churn Analysis/
│
├── Churn Analysis - EDA.ipynb
├── Churn Analysis - Model Building.ipynb
├── app.py
├── model.sav
├── templates/
│   └── home.html
└── README.md

````

---

## 📊 Exploratory Data Analysis
- Identified churn patterns based on:
  - Contract type
  - Monthly charges
  - Internet service
  - Tenure
  - Payment method
- Visualized distributions and correlations

📌 **Notebook:** `Churn Analysis - EDA.ipynb`

---

## 🤖 Model Building
- Performed feature engineering using `pd.get_dummies`
- Handled class imbalance using **SMOTEENN**
- Trained multiple models and selected:
  - ✅ **Random Forest Classifier**
- Evaluated using:
  - Confusion Matrix
  - Accuracy, Precision, Recall

📌 **Notebook:** `Churn Analysis - Model Building.ipynb`

---

## 🚀 Model Deployment
- Trained model saved as `model.sav`
- Flask API created to serve predictions
- User inputs collected from web UI
- Prediction returned as churn / non-churn

📌 **Backend:** `app.py`

---

## ▶️ How to Run the Project

### Step 1: Create & Activate Environment
```bash
conda create -n churn_env python=3.10
conda activate churn_env
````

### Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 3: Run Flask App

```bash
python app.py
```

### Step 4: Open Browser

```
http://127.0.0.1:5000/
```

---

## 📌 Output

* User enters customer details
* Model predicts whether the customer is **likely to churn or not**

---

## 📈 Future Enhancements

* Deploy on cloud (Heroku / AWS)
* Add probability-based churn score
* Improve UI with Streamlit or React


---

# 📦 requirements.txt (Create this file)

Create a new file named **`requirements.txt`** in your project folder and paste this:

```txt
flask
pandas
numpy
scikit-learn
imbalanced-learn
matplotlib
seaborn
````

If you want **exact versions (recommended)**:

```txt
flask==2.3.3
pandas==2.0.3
numpy==1.24.4
scikit-learn==1.3.2
imbalanced-learn==0.11.0
matplotlib==3.7.2
seaborn==0.12.2
```

---

