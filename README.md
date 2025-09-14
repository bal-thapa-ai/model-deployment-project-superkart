# 🛒 SuperKart – Sales Forecasting & Model Deployment  

SuperKart is a machine learning project designed to **forecast supermarket sales** and provide actionable insights for inventory planning, pricing, and regional sales strategies. The project demonstrates an **end-to-end ML workflow**: EDA → Modeling → Hyperparameter Tuning → Deployment.  

---

## 📌 Project Overview  
- Performed **Exploratory Data Analysis (EDA)** to validate data quality and uncover demand patterns.  
- Built models including **Linear Regression, Random Forest, and XGBoost**.  
- Optimized performance using **cross-validation** and **RandomizedSearchCV**.  
- Ensured **train–serve parity** by serializing preprocessing + model into a single pipeline (`pipeline.joblib`).  
- Containerized and deployed using **Flask, Gunicorn, and Docker** on **Hugging Face Spaces**.  
- Delivered insights for **inventory optimization, regional targeting, and pricing strategies**.  

---

## 🚀 Tech Stack  
- **Languages & Libraries**: Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost  
- **MLOps & Deployment**: Flask, Gunicorn, Docker, Hugging Face Spaces  
- **Techniques**: EDA, Model Evaluation, Hyperparameter Tuning, Cross-Validation, Model Serialization  

---

## 📊 Key Results  
- Accurate quarterly sales forecasting across outlets.  
- Batch and single prediction endpoints:  
  - `/predict` → Batch predictions  
  - `/v1/predict` → Single predictions with product & store IDs  
- Insights translated into **real business actions** for inventory and pricing.  

---

## 📂 Repository Structure  
```plaintext
SuperKart/
│── notebooks/           # Jupyter notebooks for EDA & model building
│── data/                # Sample dataset (cleaned for demo)
│── model/               # Serialized pipeline.joblib
│── api/                 # Flask app for deployment
│── requirements.txt     # Dependencies
│── Dockerfile           # Containerization
│── README.md            # Documentation


## 🌟 Highlights
- End-to-end pipeline: From raw data → ML model → cloud deployment.
- MLOps best practices: Train–serve parity, serialized pipelines, containerization.
- Deployment ready: Easily extensible to cloud platforms (Hugging Face, Render, Azure).
