# 🏠 House Price Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=for-the-badge&logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

> A machine learning project that predicts house prices based on property features such as area, number of rooms, location, and condition — using Linear Regression and Gradient Boosting Regressor.

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

Predicting house prices is a classic and practical regression problem in machine learning. This project builds and compares two regression models to estimate the price of a house based on structural and location-based features. The project covers the full ML pipeline — from data cleaning and EDA to model evaluation and feature importance analysis.

---

## 📊 Dataset

- **File:** `House Price Prediction Dataset.csv`
- **Samples:** 2,000 houses
- **Target:** `Price` (house price in USD)
- **Key Features:**

| Feature | Type | Description |
|---|---|---|
| `Area` | Numeric | Total area of the house (sq ft) |
| `Bedrooms` | Numeric | Number of bedrooms |
| `Bathrooms` | Numeric | Number of bathrooms |
| `Floors` | Numeric | Number of floors |
| `YearBuilt` | Numeric | Year the house was built |
| `Location` | Categorical | Downtown / Suburban / Rural |
| `Condition` | Categorical | Excellent / Good / Fair |
| `Garage` | Categorical | Yes / No |

---

## 📁 Project Structure

```
house-price-prediction/
│
├── data/
│   └── House Price Prediction Dataset.csv   # Raw dataset
│
├── notebooks/
│   └── house_price_prediction.ipynb         # Full analysis + modeling notebook
│
├── outputs/
│   ├── lr_predictions_scatter.png           # Linear Regression predictions plot
│   └── gb_predictions_scatter.png           # Gradient Boosting predictions plot
│
├── requirements.txt
└── README.md
```

---

## 🧠 Models & Techniques

### Models Applied

- ✅ **Linear Regression** *(Baseline)*
- ✅ **Gradient Boosting Regressor** *(Primary)*

### Techniques Used

| Step | Description |
|---|---|
| 🧹 Data Cleaning | Checked for missing values (none found), removed irrelevant columns (`Id`) |
| 📈 EDA | Price distribution histogram, correlation heatmap |
| 🔤 Label Encoding | Encoded `Location`, `Condition`, and `Garage` columns |
| ⚖️ Feature Scaling | Applied `StandardScaler` to normalize features |
| ✂️ Train/Test Split | 80% training, 20% testing (`random_state=42`) |
| 🤖 Model Training | Trained both Linear Regression and Gradient Boosting |
| 📉 Evaluation | MAE, RMSE, R² Score |
| 🌟 Feature Importance | Identified top predictive features from Gradient Boosting |

---

## 📈 Key Results

### Model Comparison

| Model | MAE | RMSE | R² Score |
|---|---|---|---|
| **Linear Regression** | ~244,420 | ~280,588 | ~-0.012 |
| **Gradient Boosting Regressor** | ~245,081 | ~283,910 | ~-0.036 |

### 🔑 Top Feature Importances (Gradient Boosting)

| Rank | Feature | Importance |
|---|---|---|
| 1 | 🏗️ Area | 44.0% |
| 2 | 📅 YearBuilt | 21.3% |
| 3 | 🚿 Bathrooms | 8.6% |
| 4 | 🛏️ Bedrooms | 8.4% |
| 5 | 📍 Location | 6.7% |
| 6 | 🏡 Condition | 6.6% |
| 7 | 🏢 Floors | 3.9% |
| 8 | 🚗 Garage | 0.5% |

**Area** and **YearBuilt** are by far the most influential factors in predicting house prices.

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/house-price-prediction.git
cd house-price-prediction
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
jupyter notebook notebooks/house_price_prediction.ipynb
```

You will see:
- Price distribution and correlation heatmap
- Model training and evaluation metrics (MAE, RMSE, R²)
- Actual vs Predicted scatter plots for both models
- Feature importance table from Gradient Boosting

---

## 📦 Requirements

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

Install all at once:

```bash
pip install -r requirements.txt
```

---

## 🛠️ Tools & Libraries

| Library | Purpose |
|---|---|
| `Python 3.8+` | Core programming language |
| `Pandas` | Data loading and manipulation |
| `NumPy` | Numerical computing |
| `Matplotlib` | Data visualization |
| `Seaborn` | Statistical plots (heatmap, histogram) |
| `Scikit-learn` | ML models, preprocessing, and evaluation |

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use, modify, and share.

---

## 🙌 Acknowledgements

- Dataset: House Price Prediction Dataset (CSV)
- Inspiration: Applying ML regression techniques to real-world real estate data

---

> ⭐ **If you found this project useful, please give it a star!** It helps others discover the project.
