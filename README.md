# Guangzhou Second-hand Housing Price Prediction Based on XGBoost

![Python](https://img.shields.io/badge/Python-3.10-blue)
![XGBoost](https://img.shields.io/badge/XGBoost-Regression-success)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-orange)
![License](https://img.shields.io/badge/License-MIT-green)

A machine learning project for predicting second-hand housing prices in Guangzhou using the XGBoost regression algorithm.

---

## 📖 Project Overview

This project uses **36,520 second-hand housing transaction records in Guangzhou** to build an XGBoost regression model for housing price prediction.

The complete machine learning workflow includes:

- Data loading and preprocessing
- Feature engineering
- One-Hot Encoding
- XGBoost regression model training
- Model performance evaluation
- Feature importance visualization
- Batch prediction for new housing listings

The model captures the nonlinear relationship between housing prices and factors such as location, school district, floor area, and building age, providing an efficient solution for real estate price estimation.

---

## 📂 Dataset

The project uses two datasets:

- **gz_housing.xlsx** — Historical housing transaction data (36,520 records)
- **gz_housing_pred.xlsx** — New housing listings for price prediction

**Prediction Target**

- House Price (万元)

---

## 🛠 Technologies

- Python
- Pandas
- NumPy
- OpenPyXL
- Matplotlib
- Scikit-learn
- XGBoost

---

## 🔍 Workflow

1. Data Loading
2. Data Preprocessing
3. Feature Encoding
4. Train/Test Split
5. XGBoost Regression Model
6. Model Evaluation
7. Feature Importance Analysis
8. Batch Housing Price Prediction

---

## 🤖 Machine Learning Model

**XGBoost Regressor**

Main hyperparameters:

- `n_estimators = 200`
- `learning_rate = 0.1`
- `max_depth = 6`
- `objective = reg:squarederror`

Training/Test split ratio:

- **80% Training**
- **20% Testing**

---

## 📊 Model Performance

| Metric | Result |
|---------|---------|
| R² Score | **0.9945** |
| RMSE | **33.29** |

The model explains approximately **99.45%** of the variance in housing prices, demonstrating excellent predictive performance.

---

## 📈 Feature Importance

The XGBoost model identifies the most influential features affecting housing prices:

- Location (District)
- School District
- Floor Area
- Building Age

Feature importance visualization helps interpret the pricing mechanism of Guangzhou's second-hand housing market.

---

## 📁 Project Structure

```text
Guangzhou-Housing-Price-Prediction
│
├── house_price_xgboost.py
├── gz_housing.xlsx
├── gz_housing_pred.xlsx
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🚀 Installation

Clone this repository

```bash
git clone https://github.com/your-username/Guangzhou-Housing-Price-Prediction.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

or

```bash
pip install pandas numpy openpyxl scikit-learn xgboost matplotlib
```

Run the project

```bash
python house_price_xgboost.py
```

---

## 📈 Results

The trained XGBoost model achieves high prediction accuracy and supports automatic valuation of new housing listings.

The project also provides feature importance visualization, helping analyze the key factors influencing housing prices.

---

## 👤 Author

**GitHub:** K1kibony

---

## 📄 License

This project is for educational and academic purposes only.
