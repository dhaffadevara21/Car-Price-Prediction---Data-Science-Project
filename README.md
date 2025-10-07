# 🚗 Used Car Price Prediction – Final Project (Data Science)

This repository contains my **Final Project for Data Science**, focusing on predicting **used car prices in Indonesia** using machine learning models. The project aims to help car dealers and individual sellers determine fair market prices, improving transparency and trust in the used car market.

---

## 📊 Background

* The **used car market in Indonesia** has grown significantly — up **180% over the last decade** (from 500,000 units in 2013 to 1.4 million units in 2023).
* Around **63% of consumers in Java prefer used cars** over new ones.
* **Pricing remains subjective**, often based on experience rather than data.

This project addresses that issue by developing a **data-driven price prediction model**.

---

## 🧩 Dataset

* **Source:** [CarDekho Dataset on Kaggle](https://www.kaggle.com/)
* **Records:** 4,340 used cars
* **Main Features:**

  * `Car Name`
  * `Year`
  * `Selling Price`
  * `Present Price`
  * `Kms Driven`
  * `Fuel Type`
  * `Seller Type`
  * `Transmission`
  * `Owner`

---

## 🔍 Exploratory Data Analysis (EDA) Insights

* **Fuel Type:** Petrol is dominant, followed by Diesel; CNG usage is minimal.
* **Seller Type:** Majority are dealers rather than individuals.
* **Transmission:** Manual transmissions dominate the dataset.
* **Ownership:** Most cars are first-hand (0 previous owners).
* **Car Age:** The market is dominated by cars aged 10–13 years.
* **Key Trend:** Older cars and higher mileage correlate with lower prices.

---

## 🤖 Machine Learning Models

| Model                 | Train R² | Test R² | Notes                                             |
| --------------------- | -------- | ------- | ------------------------------------------------- |
| **Linear Regression** | 0.86     | 0.87    | Strong performance, balanced, and no overfitting. |
| **Ridge Regression**  | 0.86     | 0.87    | Stable and well-regularized performance.          |
| **Random Forest**     | 0.96     | 0.78    | Overfitting observed (train too high).            |
| **Gradient Boosting** | 1.00     | 0.75    | Overfits training data heavily.                   |

✅ **Best Model:** **Linear Regression**
It provides a balance between interpretability, performance, and stability.

---

## 📈 Cross-Validation

* **Mean CV Score:** 0.81
* Consistent results across folds → reliable generalization.

---

## 💡 Key Takeaways

* **High R² (≈ 0.87)** indicates that the model explains ~87% of price variance.
* **No significant overfitting** (train ≈ test performance).
* **Simple models (Linear/Ridge)** outperform complex ones in real-world usability.

---

## 🚀 Business Implications

### 1. Fair Pricing

Helps dealers and individuals set optimal buy/sell prices aligned with market data.

### 2. Consumer Trust

Provides transparent price comparisons → **Fair / Overpriced / Good Deal** labels.

### 3. Market Segmentation

Dealers can segment inventory:

* Newer + automatic cars → higher margin.
* Older + manual cars → budget segment.

### 4. Digital Integration

Integrate price prediction into **online car trading platforms** for instant valuation.
