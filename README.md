![Thyroid](https://github.com/user-attachments/assets/02a028eb-61a5-4af6-b304-439985cd0b71)

# **Thyroid Disease Prediction** 🧬🩺

A machine learning project developed to predict the **recurrence of well-differentiated thyroid cancer** using patient clinical and pathological data. This project aims to assist healthcare professionals in making data-driven decisions through predictive analytics.

## 📊 Project Overview

This healthcare analytics project leverages classification models to identify high-risk patients using 15 years of retrospective data. It includes:

- End-to-end pipeline from **EDA**, **preprocessing**, **modeling**, to **deployment**
- Interactive **Power BI dashboard**
- Ready-to-use **model prediction interface**



## 🔍 Key Features
- Exploratory Data Analysis (EDA) on demographics, tumor characteristics, and risk factors

- Data preprocessing: missing value handling, encoding categorical features, and scaling numerical features

- Model building using:
  - Logistic Regression
  - Support Vector Classifier
  - Random Forest (Best Model: 98.7% Accuracy)
  - Gradient Boosting, Bagging, and SGD Classifier

- Hyperparameter tuning for Random Forest
- Model deployment: save/load with `joblib`, single prediction interface
- `Power BI Dashboard` for visual analytics

## 📈 Model Performance



| Model                   | Accuracy |
|------------------------|----------|
| Logistic Regression     | 97.4%    |
| SGD Classifier          | 94.8%    |
| Support Vector Classifier (SVC) | 96.1% |
| **Random Forest (Best)** | **98.7%** |
| Gradient Boosting       | 97.4%    |
| Bagging Classifier      | 97.4%    |


- **Best Model:** Random Forest
- **Accuracy:**  **__98.7%__**
- **Precision/Recall/F1:** High across all metrics
- **Top Predictive Features:** Stage, Pathology Type, Age, Focality, Radiotherapy History

## 📊 Power BI Dashboard (Visual Analytics)
This project includes a Power BI dashboard that provides interactive visualizations of the dataset. It helps users easily explore patterns related to thyroid cancer recurrence.

📌 Interactive dashboard includes:
- Demographics & Patient History
- Clinical Examination & Diagnosis
- Cancer Staging & Treatment Response
- Recurrence heatmaps and slicers by age, gender, pathology, etc.

📁 Power BI file: [`dashboards/thyroid_dashboard.pbix`](./dashboards/thyroid_dashboard.pbix)


## 🏥 Use Cases

This predictive model can be effectively integrated into **Clinical Decision Support Systems (CDSS)** to enhance healthcare delivery in the following ways:

- 🎯 Identify high-risk patients for follow-up
- 🧩 Personalized treatment strategies
- 🏥 Hospital resource optimization



## 🔮 Single Patient Prediction Module

This module allows clinicians or users to input a single patient's clinical profile and receive a prediction on whether thyroid cancer is likely to recur.

**📥 Example Input Format:**

![Example of Input Format](https://github.com/user-attachments/assets/80a6df29-2829-4283-9847-78eaca4b0e0f)

**⚙️ How It Works**
- **Input is received** in dictionary format.

- **Categorical values are encoded** using `OneHotEncoder`.

- **Numerical values (Age)** are scaled using `MinMaxScaler`.

- **Features are combined** into a prediction-ready format.

- **Random Forest model** predicts:

  - ✅ Prediction (`Yes` / `No` for recurrence)

  - 📊 Probability score (confidence level)



**🧠 Prediction Function**

![Prediction Function](https://github.com/user-attachments/assets/58968d5a-6965-40b0-848f-f3729d9426e3)


**📌 Output**

![Output](https://github.com/user-attachments/assets/f5a4c610-c209-443d-9a41-187669499aa3)

This means the patient is **unlikely to experience recurrence**, with a **97.9%** confidence level.
## 🛠️ Tech Stack

- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Plotly)
- Power BI for visualization
- Jupyter Notebook
- `joblib` for model serialization

## 📄 Reports

A detailed project report is included in [`/reports/Thyroid_Disease_Prediction_Report.pdf`](./dashboards/thyroid_dashboard.pbix), covering methodology, model performance, results, and recommendations.
