---

# 📊 Customer Churn Analysis & Prediction

This project focuses on **end-to-end customer churn analysis**, including **Exploratory Data Analysis (EDA)**, **machine learning model building**, and **deployment of the final model using a Flask web application**.

The goal is to identify customers who are more likely to churn and help businesses take proactive retention actions.

---

## 🚀 Project Overview

Customer churn is a major challenge for subscription-based businesses.
In this project, we:

* Performed **Exploratory Data Analysis (EDA)** to understand churn behavior
* Identified key factors influencing customer churn
* Built a **Machine Learning model** using **Random Forest Classifier**
* Handled class imbalance using **SMOTEENN**
* Deployed the trained model using a **Flask API**
* Created a simple **frontend UI** to get churn predictions

---

## 🧠 Machine Learning Workflow

1. **Data Cleaning & Preprocessing**

   * Handling missing values
   * Encoding categorical variables using `pd.get_dummies`
   * Feature engineering (tenure grouping, etc.)

2. **Exploratory Data Analysis**

   * Churn distribution analysis
   * Feature-wise churn impact
   * KDE plots, bar plots, and correlation analysis

3. **Handling Imbalanced Data**

   * Used **SMOTEENN** to balance churn and non-churn classes

4. **Model Building**

   * Random Forest Classifier
   * Model evaluation using accuracy, confusion matrix, and ROC-AUC

5. **Model Saving**

   * Final trained model saved as `model.sav`

---

## 🛠️ Technologies Used

* Python 3.10
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn (SMOTEENN)
* Flask
* HTML (Frontend)

---

## 📂 Project Structure

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
```

---

## 🌐 Flask Application Details

* **GET /**
  Loads the home page (`home.html`)

* **POST /**
  Accepts customer details from the frontend and returns churn prediction

Run the Flask app using:

```
python app.py
```

The app will be available at:

```
http://127.0.0.1:5000/
```

---

## ▶️ How to Run the Project

1. Create a virtual environment:

```
conda create -n churn_env python=3.10
conda activate churn_env
```

2. Install dependencies:

```
pip install flask pandas numpy scikit-learn imbalanced-learn matplotlib seaborn
```

3. Navigate to the project folder:

```
cd "S:\DataAnalystProjects\Customer Churn Analysis"
```

4. Run the Flask app:

```
python app.py
```

5. Open browser and visit:

```
http://127.0.0.1:5000/
```

---

## 📈 Model Output

The model predicts:

* **Churn = Yes** → Customer is likely to leave
* **Churn = No** → Customer is likely to stay

---

## 🎯 Key Learnings

* Importance of EDA in understanding customer behavior
* Handling imbalanced datasets using SMOTEENN
* End-to-end ML pipeline from data analysis to deployment
* Practical experience with Flask-based ML deployment

---

## 📌 Future Improvements

* Add model explainability (SHAP / Feature Importance)
* Improve frontend UI
* Deploy on cloud (Heroku / Render / AWS)
* Add logging and exception handling

---

