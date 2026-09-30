# 🏠 Real Estate Listing Classifier

### Ensemble Text & Visual Anomaly Detection for Authentic Real Estate Listings

A Machine Learning project developed to identify potentially **fake or misleading real-estate listings** using property-related information.

## 📌 Overview

The project analyzes real-estate data such as price, location, property size, amenities, and other attributes to classify listings as **Real or Fake**.

The workflow combines **Extra Trees feature selection** with an **Artificial Neural Network (MLP)** for classification.

## 🎯 Objectives

* Detect potentially fake real-estate listings
* Clean and preprocess data
* Handle missing and categorical values
* Select important features using Extra Trees
* Classify listings using ANN/MLP
* Evaluate model performance

## 📊 Dataset

| Property       | Value |
| -------------- | ----: |
| Records        | 2,452 |
| Columns        |    21 |
| Real Listings  | 2,154 |
| Fake Listings  |   298 |
| Input Features |    19 |

## 🔄 Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Preprocessing
   ↓
Feature Encoding & Scaling
   ↓
Extra Trees Feature Selection
   ↓
ANN / MLP Classification
   ↓
Model Evaluation
```

## 📈 Evaluation

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* ROC Curve

**Recorded Accuracy: 87.17%**

> The dataset is imbalanced, so accuracy alone should not be used to judge model performance.

## 🛠️ Technologies

**Python • Pandas • NumPy • Scikit-learn • Matplotlib • Seaborn • Joblib • Jupyter Notebook**

## 📂 Project Structure

```text
Real_Estate_Listing_Classifier/
├── source_code/
├── dataset/
├── model/
├── results/
├── Project_Report.pdf
├── requirements.txt
└── README.md
```

## 🚀 Future Scope

* Handle class imbalance
* Improve minority-class performance
* Add NLP for listing descriptions
* Add image-based analysis
* Deploy as a web application/API

## 📜 Conclusion

This project demonstrates an end-to-end Machine Learning workflow for detecting potentially fake real-estate listings using **Extra Trees feature selection and ANN/MLP classification**.
