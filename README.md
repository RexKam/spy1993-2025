# 📈 SPY 1993-2025 Analysis

This project uses Python and Jupyter Notebook to analyze the historical daily trading data of SPY (S&P 500 ETF) from 1993 to 2025. The notebook covers data preprocessing, feature exploration, visualization, and regression modeling for predicting closing prices.

## 📂 Contents

- `spy1993-2025.ipynb`: Main analysis notebook with all code, visualizations, and results.
- `spy.csv`: Historical SPY dataset (required to run the notebook).

## 🔗 Data Source

- The historical SPY data used in this project comes from Kaggle:  
  [S&P 500 (SPY) Dataset on Kaggle](https://www.kaggle.com/datasets/gkitchen/s-and-p-500-spy/data)

## 🛠️ Features

- **Data Exploration**  
  - Load and inspect SPY price data from 1993 to 2025
  - Visualize feature relationships with pairplots and time series plots

- **Feature Engineering**  
  - Analyze correlations between Open, High, Low, Close, and Volume
  - Add derived columns (day, weekday, week, month, year) for further analysis

- **Modeling**  
  - Predict closing prices using polynomial regression
  - Use cross-validation (KFold, GridSearchCV) to select the best polynomial degree
  - Report the best model and its mean squared error (MSE)

## ⭐ Key Findings

- Price-related features have clear correlations
- The best model for closing price prediction is linear regression (polynomial degree = 1)
- Increasing model complexity does not significantly improve prediction accuracy

## ▶️ How to Run

1. Clone this repository.
2. Ensure you have Python and the following packages installed:
    - pandas
    - numpy
    - matplotlib
    - seaborn
    - scikit-learn
3. Place `spy.csv` in the same directory as the notebook.
4. Open `spy1993-2025.ipynb` in Jupyter Notebook or Google Colab.
5. Run all cells to reproduce the analysis and visualizations.

## 🖼️ Example Visualizations

- Pairplot of feature correlations
- Time series plot of closing prices

## 📝 Conclusion

The closing price of SPY can be effectively predicted using a linear relationship with open, high, low, and volume features. Increasing model complexity does not bring significant accuracy improvements. For more advanced forecasting, consider adding technical indicators, macroeconomic data, or non-linear machine learning models.

