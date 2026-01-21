# 🧠 Money Laundering Transaction Detection using Machine Learning Algorithms

An end-to-end machine learning project that detects **suspicious financial transactions** using supervised machine learning models. The project combines exploratory analysis, model development, threshold optimization, and an interactive dashboard to support **practical Anti-Money Laundering (AML) decision-making**.

---

## 🔍 Project Overview

Money laundering remains a major global financial crime. This project applies machine learning to improve detection accuracy while maintaining interpretability and operational relevance.

Using a realistic **synthetic AML transaction dataset**, the project builds and compares **Random Forest** and **XGBoost** models, applies **threshold tuning** to handle class imbalance, and visualizes results through an interactive dashboard tailored for stakeholders.

---

## 🎯 Objectives

* Explore transaction patterns through **EDA and feature analysis**
* Build and evaluate ML classifiers to detect suspicious transactions
* Address **class imbalance** using sampling strategies and threshold tuning
* Compare model performance using **precision, recall, F1-score, and accuracy**
* Identify **key risk-driving features** via feature importance analysis
* Communicate findings using a **business-focused dashboard**

---

## 📦 Dataset

* **Synthetic Anti-Money Laundering Dataset (SAML-D)**
* Publicly available on [Kaggle](https://www.kaggle.com/datasets/berkanoztas/synthetic-transaction-monitoring-dataset-aml)
* Simulates realistic transaction behaviors while protecting sensitive information

> Note: The dataset is not included in this repository due to size and reproducibility considerations.

---

## 🧪 Machine Learning Approach

### Models Implemented

* **Random Forest**
* **XGBoost**

### Key Techniques

* Stratified train / validation / test split (70 / 15 / 15)
* Feature engineering and categorical encoding
* Handling class imbalance during training
* Hyperparameter tuning using Randomized Search
* **Probability threshold optimization** to balance recall and false positives

### Model Selection

Random Forest emerged as the preferred model due to:

* Strong and stable **F1-score**
* Fewer false positives
* Better recall compared to XGBoost under optimized thresholds

---

## 📊 Dashboard & Business Analytics

An interactive dashboard was developed to translate model outputs into insights for non-technical stakeholders.

### Dashboard Capabilities

* Overall transaction and laundering trend analysis
* High-risk transaction typologies and payment types
* Geographic risk patterns (pair bank locations)
* Model prediction summaries and performance indicators
* Descriptive, diagnostic, predictive, and prescriptive analytics

📄 **Dashboard (PDF)**
➡️ `dashboard/AML_Dashboard.pdf`

---

## 🗂 Repository Structure

```text
money-laundering-detection-ml/
│
├── README.md
├── notebooks/
│   ├── 01_data_preparation_eda.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_model_training_evaluation.ipynb
│   └── 04_threshold_optimization.ipynb
│
├── dashboard/
│   ├── AML_Dashboard.pdf
│
├── slides/
│   └── Money_Laundering_Detection_Presentation.pdf

```

---

## 🚀 Key Results & Insights

* Machine learning significantly reduces reliance on traditional rule-based systems
* Threshold tuning proved effective in managing **imbalanced AML data**
* Laundering transactions are rare but typically involve **larger transaction amounts**
* Structural and monetary features contribute more to predictions than temporal features
* Random Forest provides a strong balance between **detection capability and stability**

---

## ⚠️ Limitations

* Synthetic data may not fully capture real-world transaction complexity
* Models focus on tabular ML; graph-based and deep learning methods are not explored
* Feature importance offers limited explainability compared to SHAP-based approaches

---

## 🔮 Future Enhancements

* Apply **SHAP** for improved model explainability
* Explore **graph-based AML models** for network-level risk detection
* Validate methodology using real institutional datasets (subject to access)
* Extend dashboard with real-time monitoring concepts

---

## 🛠 Tools & Technologies

* Python (Pandas, NumPy, Scikit-learn, XGBoost)
* Jupyter Notebook / Google Colab
* Power BI
* Machine Learning & Statistical Evaluation Metrics

---

