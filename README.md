

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

This notebook serves as a great starting point for supervised regression problems using real-world data. The dataset is clean, the features are interpretable, and the results are a solid benchmark for beginners.
