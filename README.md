Gold Price Prediction using Random Forest Regressor 🪙📈

This project builds a Machine Learning regression model to predict **Gold ETF price (GLD)** using financial market indicators such as:

✔ S&P 500 Index (SPX)  
✔ Oil Price (USO)  
✔ Silver Price (SLV)  
✔ EUR/USD Exchange Rate  

The model is trained using **Random Forest Regressor** and evaluated using the **R² Score**.

📊 Dataset Information

File: `gld_price_data.csv`

• Total Rows: **2290**  
• Total Columns: **6**  
• Dataset contains **no missing values**

| Column | Description |
|-------|-------------|
| Date | Trading date |
| SPX | S&P 500 index value |
| GLD | Gold ETF price (Target) |
| USO | Oil ETF price |
| SLV | Silver ETF price |
| EUR/USD | Currency exchange rate |

🎯 Project Objective

Predict **Gold Price (GLD)** using market indicators:

- SPX
- USO
- SLV
- EUR/USD

🧰 Libraries Used

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

⚙️ Project Workflow

📥 Data Loading  
• Import dataset using Pandas  
• Inspect rows, columns, statistics, and missing values  

📈 Exploratory Data Analysis (EDA)  
• Correlation matrix analysis  
• Heatmap visualization  
• Distribution analysis of GLD prices  

💡 Key Insights
- SLV → Strong positive correlation with gold price
- USO → Negative correlation
- SPX & EUR/USD → Weak correlation

🧩 Feature Engineering

Features (X):
- SPX
- USO
- SLV
- EUR/USD

Target (Y):
- GLD

✂️ Train–Test Split

• Training Data: 80%  
• Testing Data: 20%  
• Random State: 2

🤖 Model Training

Model Used:
**RandomForestRegressor**

Parameter:
- `n_estimators = 100`

📏 Model Evaluation

Metric Used:
✅ R² Score

Result:
⭐ **R² Score = 0.9891**

The model shows very high predictive accuracy.
📉 Visualization

Comparison Plot:
• Actual Gold Prices  
• Predicted Gold Prices  

Helps visually evaluate model performance.

🏆 Results & Insights

✔ Random Forest captures complex non-linear relationships  
✔ Ensemble learning reduces overfitting  
✔ High prediction accuracy achieved

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
