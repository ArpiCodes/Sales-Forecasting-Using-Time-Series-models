# 📊 *Sales Forecasting Using Time Series Models*

## 🌟 *Project Overview*

This project focuses on sales forecasting across categories and regions using advanced time series models—ARIMA, Prophet, and SARIMA. The performance of these models has been evaluated using Root Mean Squared Error (RMSE) and Mean Absolute Percentage Error (MAPE). ARIMA serves as the baseline model, and the results highlight improvements brought by Prophet and SARIMA.

The analysis identifies the most suitable models for capturing seasonal patterns, trend sensitivity, and overall accuracy, providing data-driven insights into sales forecasting.

📈 From *trends* to *seasonal patterns*, the results highlight:  
- The strengths of *Prophet* in capturing trends.  
- The precision of *SARIMA* in seasonal forecasting.  
- Why *ARIMA* works as a baseline but not the best choice for production.  

With *RMSE* and *MAPE* as benchmarks, we deliver actionable insights for *categories* (Furniture, Office Supplies, Technology) and *regions* (Central, East, South, West).

---

## 🎯 *Project Goals*

- 🧠 Build and Evaluate Models: Develop ARIMA, Prophet, and SARIMA models for sales forecasting.
- 🔬 Category- and Region-Wise Comparison: Evaluate forecasting performance across sales categories (Furniture, Office Supplies, Technology) and regions (Central, East, South, West).
- 📊 Quantify Model Improvements: Compare Prophet and SARIMA against ARIMA using RMSE and MAPE.
- 🕵 Error Analysis: Examine residuals to understand model-specific deviations and trends.
- 💡 Model Recommendations: Identify the best models for different forecasting needs.

---

## 🔥 *Why This Project Matters*

In today's competitive market, *forecast accuracy* is critical for:  
✔ Reducing inventory waste.  
✔ Meeting customer demands.  
✔ Enhancing operational efficiency.  

This project equips businesses with the tools and insights to stay ahead by:  
- Detecting *patterns* and *anomalies* in sales trends.  
- Leveraging the best-fit models for *seasonality* or *trend-focused predictions*.

---

## ✨ *Key Highlights*

### 📌 *1. Model Performance At a Glance*
- **🌊 SARIMA**: Best-performing model for region-wise forecasting, capturing seasonal patterns with lower error variance.
- **🔮 Prophet**: Best-performing model for category-wise forecasting, demonstrating strong trend sensitivity and accuracy.
- **📊 ARIMA**: Baseline model with consistently higher RMSE and MAPE.
  

### 📊 *2. Category-Specific Performance*
| Category | 🧪 Prophet | 🌊 SARIMA | 📊 ARIMA | 🥇 Best Model |
|----------|-----------|-----------|----------|--------------|
| 🛋 Furniture | RMSE: 4,423.56<br>MAPE: 23.72% | RMSE: 5,681.29<br>MAPE: 24.61% | RMSE: 10,117.36<br>MAPE: 33.78% | Prophet |
| 📋 Office Supplies | RMSE: 6,755.30<br>MAPE: 22.82% | RMSE: 5,872.83<br>MAPE: 25.96% | RMSE: 9,363.07<br>MAPE: 32.00% | Prophet |
| 💻 Technology | RMSE: 8,182.96<br>MAPE: 28.24% | RMSE: 9,649.08<br>MAPE: 33.11% | RMSE: 13,513.31<br>MAPE: 31.72% | Prophet |
---

### 🌍 *3. Regional-specific Performance*
| Region | 🧪 Prophet | 🌊 SARIMA | 📊 ARIMA | 🥇 Best Model |
|--------|-----------|-----------|----------|--------------|
| 🏛 Central | RMSE: 5,259.02<br>MAPE: 55.32% | RMSE: 9,802.91<br>MAPE: 104.36% | RMSE: 4,822.81<br>MAPE: 56.44% | ARIMA |
| 🌅 East | RMSE: 9,034.83<br>MAPE: 51.23% | RMSE: 11,560.50<br>MAPE: 37.88% | RMSE: 13,690.42<br>MAPE: 48.69% | Prophet |
| 🍃 South | RMSE: 8,045.62<br>MAPE: 52.26% | RMSE: 7,684.45<br>MAPE: 42.19% | RMSE: 7,857.68<br>MAPE: 44.29% | SARIMA |
| 🌄 West | RMSE: 5,502.32<br>MAPE: 17.63% | RMSE: 4,744.49<br>MAPE: 15.81% | RMSE: 9,134.87<br>MAPE: 28.72% | SARIMA |
---

### 📉 *4. Model Improvement Over ARIMA*

### 📦 Category Improvements

| Category | 🧪 Prophet RMSE Improvement | 🌊 SARIMA RMSE Improvement |
|----------|----------------------------|----------------------------|
| 🛋 Furniture | 56.28% | 43.85% |
| 📋 Office Supplies | 27.85% | 37.28% |
| 💻 Technology | 39.45% | 28.60% |

### 🗺 Region Improvements

| Region | 🧪 Prophet RMSE Improvement | 🌊 SARIMA RMSE Improvement |
|--------|----------------------------|----------------------------|
| 🏛 Central | -9.04% (worse than ARIMA) | -103.26% (worse than ARIMA) |
| 🌅 East | 34.01% | 15.56% |
| 🍃 South | -2.39% (worse than ARIMA) | 2.20% |
| 🌄 West | 39.77% | 48.06% |
---

## 🔍 Model Insights

### 🧠 Error Analysis

- *🔮 Prophet*: 
  - Effective at capturing trends but showed occasional residual variability.
- *🌊 SARIMA*: 
  - Strong in handling seasonal patterns, with lower RMSE and MAPE than ARIMA.
- *📊 ARIMA*: 
  - Consistently higher residuals, making it unsuitable for accurate forecasting.

## 🚀 *Installation and Usage*

### 📋 *Requirements*
- *🐍Python*: Version 3.8+  
- *📚Libraries*:
   - pandas
   - numpy
   - statsmodels
   - prophet
   - matplotlib
   - seaborn  

### ⚙ *Setup Instructions*
1. *Clone the repository*:  
   ```bash
   git clone https://github.com/ArpiCodes/sales-forecasting-time-series.git
   ```
   
2. *Navigate to the project folder*:  
   ```bash
   cd sales-forecasting-time-series
   ```
   
3. *Install required libraries*:  
   ```bash
   pip install -r requirements.txt
   ```
   

### ▶ *How to Run the Code*
1. Add your dataset to the data/ folder.  
2. Open the Jupyter Notebook:  
   ```bash
   jupyter notebook notebooks/sales_forecasting.ipynb
   ```
   
3. Run the notebook to explore:  
   - Model metrics (RMSE, MAPE).  
   - Comparative performance visualizations.  
   - Residual error analysis.

---

## 📂 *Project Structure*
```
sales-forecasting-time-series/
├── data/
│   └── sales_data.csv          # Input dataset
├── notebooks/
│   └── sales_forecasting.ipynb # Main notebook
├── results/
│   ├── model_metrics.csv       # RMSE & MAPE metrics
│   └── improvement_analysis.csv # Improvement analysis
├── README.md                   # Project documentation
└── requirements.txt            # Dependencies list
```

---

## 🏆 *Key Insights*
- *📈 Category-Wise Forecasting*:
  - Best Model: Prophet (lowest RMSE and MAPE across categories).
  - Ideal for applications requiring trend-sensitive forecasting.
- *🌐 Region-Wise Forecasting*:
  - Best Model: SARIMA (lowest RMSE and error variance across regions).
  - Suitable for scenarios with pronounced seasonality.
- *📊 Baseline*: ARIMA provides a benchmark but is not recommended for production use.

---

## 🙏 *Acknowledgments*
- *📈 ARIMA*: Statistical approach for time series analysis.
- *🔮 Prophet*: Developed by Facebook for scalable forecasting.
- *🌊 SARIMA*: Seasonal Autoregressive Integrated Moving Average model.

