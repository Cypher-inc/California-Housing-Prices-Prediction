

# 🏡 California Housing Price Prediction

This project involves **Exploratory Data Analysis (EDA)**, **feature encoding**, and **model training** on the **California Housing** dataset. The aim is to predict median house values based on various socio-economic and geographic features.

---

## 📁 Project Structure

- `californiaHousingMain.ipynb`: Main Jupyter notebook containing:
  - Data loading and inspection
  - Exploratory Data Analysis (EDA)
  - Encoding categorical variables
  - Train-test splitting
  - Regression model training and evaluation

---

## 📊 Dataset

- Source: `housing.csv` from the [California Housing Dataset](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html)
- Features include:
  - Median income
  - Housing age
  - Average rooms and bedrooms
  - Population
  - Latitude and longitude
  - Ocean proximity (categorical)

---

## ⚙️ Models Used

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor (or other models depending on final implementation)

---

## 📈 Key Takeaways

- EDA reveals correlations and distribution of features
- Missing values handled effectively
- After model tuning and training, predictions are compared using appropriate evaluation metrics (e.g., RMSE or R²)

---

## 🧪 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Cypher-inc/California-Housing-Prices-Prediction.git
   cd california-housing
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook:
   ```bash
   jupyter notebook californiaHousingMain.ipynb
   ```
   
---

## 📌 Conclusion

### Model Performance Summary

| Model            | Dataset | R² Score | RMSE      |
|------------------|---------|----------|-----------|
| **Linear**       | Train   | 0.628    | 55,736.59 |
|                  | Test    | 0.628    | 55,736.59 |
| **SVR**          | Train   | -0.025   | 93,390.27 |
|                  | Test    | -0.023   | 92,454.27 |
| **RBF SVR**      | Train   | -0.025   | 93,390.27 |
|                  | Test    | -0.023   | 92,454.27 |
| **Decision Tree**| Train   | 1.000    | 0.00      |
|                  | Test    | 0.538    | 62,137.55 |
| **Random Forest**| Train   | 0.969    | 16,183.10 |
|                  | Test    | 0.793    | 41,635.08 |
| **XGBoost**      | Train   | 0.855    | 35,158.88 |
|                  | Test    | 0.798    | 41,051.61 |


- 🔹 **XGBoost**  performed the best overall, with high R² scores and relatively low RMSE on both train and test sets.
- 🔹 **Random Forest and Decision Tree** overfit the training data (R² = 0.96 - 1.0), resulting in weaker generalization.
- 🔸 **SVR** models underperformed, with negative R² values indicating they failed to capture variance in the data.

