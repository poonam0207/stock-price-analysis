# 📈 MasterCard Stock Price Analysis

This project provides a time series analysis and trading signal generation based on MasterCard's historical stock prices from 2005 to 2011. The analysis includes data preprocessing, statistical metrics, visualizations, and a simple moving average-based trading strategy.
Data source: https://www.kaggle.com/datasets/mayankanand2701/mastercard-stock-price-dataset

## 🔧 Requirements

Make sure you have the following Python libraries installed:

```bash
pip install pandas numpy matplotlib
```

## 📁 Files

- `MasterCard Stockt price Analysis.py`: The main Python script containing data loading, processing, visualization, and analysis.
- `Mastercard Dataset.csv`: CSV file containing historical stock data of MasterCard.

## 📊 Analysis Overview

### 1. 📥 Data Loading and Preparation
- Reads the CSV file into a DataFrame.
- Converts the `Date` column to datetime format and sets it as the index.
- Checks for missing values and duplicates.

### 2. 📉 Time Series Plot
- Plots the daily closing price from 2005 to 2011.

### 3. 🔁 Daily Returns
- Calculates and plots daily percentage returns (`Close` price).
- Displays histogram to understand volatility.

### 4. 📈 Moving Averages
- Calculates 50-day and 200-day simple moving averages (SMA).
- Visualizes SMAs over time alongside the closing price.

### 5. 📆 Monthly and Yearly Trends
- Resamples and plots average monthly and yearly closing prices.

### 6. 🧮 Key Metrics
- Highest and lowest closing prices.
- Total return over the dataset period.
- Average daily volume.

### 7. 🔗 Correlation Analysis
- Calculates and displays correlation matrix between `Open`, `High`, `Low`, and `Close`.

### 8. 🛎️ Trading Signal (Golden Cross Strategy)
- A basic strategy using SMA crossover:
  - Signal = 1 when 50-day SMA > 200-day SMA (buy signal).
- Plots buy signals on the price chart.

## 📌 How to Use

1. Place the `Mastercard Dataset.csv` in the same directory as the script.
2. Run the Python script:
   ```bash
   python "MasterCard Stockt price Analysis.py"
   ```

## 📷 Sample Output

- Closing price trends
- Daily return volatility
- Monthly/yearly average trends
- SMA crossover trading signals

## 📎 Notes

- The trading strategy implemented is simplistic and does not account for transaction costs or risk management.
- Yearly resampling incorrectly uses `'M'` (monthly) instead of `'Y'` – you may want to correct that in the code.

## 📬 Contact

For questions or enhancements, feel free to raise an issue or contribute!
