# ❤️ Heart Disease Prediction

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=for-the-badge&logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

> A machine learning project that predicts whether a person is at risk of heart disease based on clinical medical data — using Logistic Regression and Decision Tree classifiers.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Models & Techniques](#models--techniques)
- [Key Results](#key-results)
- [Installation](#installation)
- [Usage](#usage)
- [Tools & Libraries](#tools--libraries)
- [License](#license)

---

## 🔍 Overview

Heart disease is one of the leading causes of death worldwide. Early detection can save lives. This project builds a **binary classification model** that predicts the presence or absence of heart disease in a patient using medical features such as chest pain type, cholesterol levels, and heart rate.

---

## 📊 Dataset

- **Source:** [Heart Disease UCI Dataset – Kaggle](https://www.kaggle.com/datasets/ronitf/heart-disease-uci)
- **Samples:** 303 patients
- **Target:** `1` = Heart Disease Present, `0` = No Heart Disease
- **Key Features:**

| Feature | Description |
|---|---|
| `cp` | Chest Pain Type |
| `thalach` | Maximum Heart Rate Achieved |
| `oldpeak` | ST Depression (Exercise vs Rest) |
| `ca` | Number of Major Vessels (Fluoroscopy) |
| `thal` | Thalassemia Type |
| `age` | Age of the Patient |
| `sex` | Sex (1 = Male, 0 = Female) |

---

## 📁 Project Structure

```
heart-disease-prediction/
│
├── data/
│   └── heart.csv                  # Raw dataset
│
├── notebooks/
│   └── heart_disease_analysis.ipynb  # Full EDA + Modeling notebook
│
├── src/
│   ├── preprocessing.py           # Data cleaning & feature scaling
│   ├── model.py                   # Model training & evaluation
│   └── visualizations.py          # Plots and charts
│
├── outputs/
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── feature_importance.png
│
├── requirements.txt
└── README.md
```

---

## 🧠 Models & Techniques

### Models Applied
- ✅ **Logistic Regression** *(Primary)*
- ✅ **Decision Tree Classifier** *(Optional/Comparison)*

### Techniques Used

| Step | Description |
|---|---|
| 🧹 Data Cleaning | Handled missing values, removed duplicates |
| 📈 EDA | Distribution plots, correlation heatmaps |
| ⚖️ Feature Scaling | StandardScaler for numerical features |
| 🤖 Classification | Trained & tuned ML models |
| 📉 ROC Curve | AUC score for model performance |
| 🔲 Confusion Matrix | Evaluated TP, TN, FP, FN |
| 🌟 Feature Importance | Identified top predictive features |

---

## 📈 Key Results

| Metric | Score |
|---|---|
| **Accuracy** | ~85%+ |
| **ROC-AUC Score** | Strong performance |
| **Precision** | High |
| **Recall** | High |

### 🔑 Most Important Features

1. 🫀 **Chest Pain Type** (`cp`)
2. 💓 **Maximum Heart Rate** (`thalach`)
3. 📉 **ST Depression** (`oldpeak`)
4. 🩻 **Number of Vessels (Fluoroscopy)** (`ca`)

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/heart-disease-prediction.git
cd heart-disease-prediction
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

### Run the Jupyter Notebook

```bash
jupyter notebook notebooks/heart_disease_analysis.ipynb
```

### Or Run the Python Script

```bash
python src/model.py
```

You will see:
- Model accuracy printed in the console
- Confusion matrix and ROC curve saved to `outputs/`
- Feature importance plot displayed

---

## 🛠️ Tools & Libraries

| Library | Purpose |
|---|---|
| `Python 3.8+` | Core programming language |
| `Pandas` | Data manipulation |
| `NumPy` | Numerical computing |
| `Matplotlib` | Data visualization |
| `Seaborn` | Statistical plots |
| `Scikit-learn` | ML models & evaluation |

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use, modify, and share.

---

## 🙌 Acknowledgements

- Dataset: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/heart+Disease) via Kaggle
- Inspiration: Using AI/ML to support early medical diagnosis

---

> ⭐ **If you found this project helpful, please give it a star!** It motivates further development.
