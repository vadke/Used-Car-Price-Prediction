# 🚗 Used Car Price Prediction & Valuation Model

## 📌 Business Overview
In the pre-owned automotive industry, pricing efficiency is key to profitability. This project builds a data-driven valuation model to predict the `Selling_Price` of used cars. By accurately estimating market value, dealerships can optimize their procurement strategy and reduce the "Days to Sell" metric.

## 📊 Technical Approach
This analysis goes beyond simple prediction by incorporating rigorous **Statistical Diagnostics** to ensure model reliability.

* **Data Source:** `car_data.csv` (Features: Year, Present Price, Kms Driven, Fuel Type, etc.)
* **Models Implemented:**
    * **Multiple Linear Regression:** (Baseline)
    * **Polynomial Regression:** (To capture non-linear depreciation curves)
    * **LazyPredict:** (AutoML for benchmarking)
* **Statistical Tests:**
    * **VIF (Variance Inflation Factor):** Used to identify and handle multicollinearity.
    * **Homoscedasticity Check:** Residuals vs. Fitted plots.
    * **Normality Check:** Q-Q Plots and Histograms of residuals.

## 📈 Key Findings
1.  **Depreciation is Non-Linear:** The Polynomial Regression model outperformed the linear model, confirming that cars depreciate faster in their early years.
2.  **Top Predictors:** The `Present_Price` (original showroom price) is the single biggest predictor of resale value, followed closely by the vehicle's age.
3.  **Diesel vs. Petrol:** Diesel cars in this dataset retained higher resale value compared to their petrol counterparts.

## 🛠 Tools Used
* **Python:** Pandas, NumPy, Statsmodels
* **Machine Learning:** Scikit-Learn, LazyPredict
* **Visualization:** Seaborn, Matplotlib

## 🚀 How to Run
1.  Clone the repository.
2.  Install dependencies: `pip install -r requirements.txt`
3.  Run `Car_Price_Prediction.ipynb`.
