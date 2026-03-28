#  Data Science Project: Market Sentiment & Trading Analysis

 Overview
This project consists of two real-world financial datasets:
1. Fear & Greed Index (market sentiment)
2. Crypto Trading Data (trading performance)

The goal is to analyze patterns, build machine learning models, and extract meaningful insights from financial data.


#  Project 1: Fear & Greed Index Analysis

##  Dataset Description
- timestamp → Unix timestamp  
- value → Sentiment score (0–100)  
- classification → Fear / Greed categories  
- date → Date  

##  Objective
- Analyze market sentiment over time  
- Predict sentiment using machine learning  

##  Steps Performed
- Data Cleaning (datetime conversion)
- Feature Engineering (year, month, day, weekday)
- Data Visualization:
  - Time series plot
  - Histogram
  - Boxplot
  - Heatmap
- Model Building:
  - Random Forest Classifier
  - Pipeline & ColumnTransformer

##  Key Insight (Important)
The initial model showed very high accuracy (~99%) due to data leakage, as the `value` directly determines the `classification`.

Fix:
- Removed leakage features  
- Used time-based features for realistic modeling  

---

#  Project 2: Crypto Trading Analysis

##  Dataset Description
- Trade details including price, size, fees, and profit/loss (PnL)

 Objective
- Analyze trading performance  
- Identify profitable strategies  
- Predict profit/loss  

 Steps Performed
- Data Cleaning  
- Feature Engineering (time-based features)  
- Data Visualization:
  - Profit over time
  - Trade distribution
  - Coin-wise performance
- Model Building:
  - Linear Regression
  - Random Forest Regressor
  - Pipeline & ColumnTransformer

 Key Insights
- Certain coins generate higher profits  
- Trading time affects profitability  
- Fees have a direct impact on PnL  

---

 Machine Learning Techniques Used
- Data Preprocessing  
- Feature Engineering  
- Pipeline (end-to-end workflow)  
- ColumnTransformer (handling different data types)  
- Random Forest (classification & regression)  
- Cross Validation  
- Hyperparameter Tuning  

---

# 📈 Results

| Model | Task | Performance |
|------|------|-----------|
| Random Forest | Classification | ~99% Accuracy (before leakage fix) |
| Random Forest | Regression | Good R² Score |


 Tools & Technologies
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

# 📁 Project Structure

project/
│
├── fear_greed/
│   ├── fear_greed_analysis.ipynb
│   └── fear_greed_index.csv
│
├── trading/
│   ├── trading_analysis.ipynb
│   └── sample_trading_data.csv
│
├── README.md

---

#  Conclusion
- Market sentiment plays a crucial role in trading behavior  
- Proper feature selection is critical to avoid data leakage  
- Machine learning pipelines ensure clean and scalable workflows  

---

#  Author
Vikesh Kumar  
B.Tech CSE Student  
Aspiring Data Scientist  
