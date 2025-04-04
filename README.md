# 📈 Stock Price Forecasting using LSTM

This project leverages Long Short-Term Memory (LSTM) neural networks to forecast Google's stock prices using 20 years of historical data. It demonstrates end-to-end implementation of time-series analysis, feature engineering, deep learning model training, evaluation, and visualization.

## 🚀 Features

- ✅ Downloaded 20 years of historical stock data for Google using `yfinance`
- 📊 Performed exploratory data analysis (EDA) including moving averages, trend plotting, and daily return computation
- 🧠 Built a sequential LSTM model using Keras with TensorFlow backend
- 📉 Evaluated model with Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² score
- 💾 Saved the trained model for future inference using `.keras` format

## 🛠️ Tech Stack

- Python 3.10+
- yfinance
- pandas
- matplotlib / seaborn
- scikit-learn
- numpy
- TensorFlow / Keras

## 📂 Directory Structure

├── stock_forecasting_lstm.ipynb # Jupyter Notebook with full implementation
├── README.md # Project documentation 
├── Latest_stock_price_model.keras# Saved LSTM model 
├── requirements.txt # Python dependencies


## 📊 Sample Visualizations

### Google Adjusted Close Price (2004–2024)
> A line plot showing historical stock performance over 20 years.

### Moving Averages
> Plots of 100-day and 250-day moving averages alongside actual prices for trend analysis.

## 🧪 Model Performance Metrics

| Metric         | Value   |
|----------------|---------|
| MAE            | 0.009   |
| RMSE           | 0.012   |
| R² Score       | 0.93    |

## 🧠 LSTM Model Architecture
Input: (100 timesteps, 1 feature) → LSTM (128 units, return_sequences=True) → LSTM (64 units, return_sequences=False) → Dense (25 units) → Dense (1 unit)


## ⚙️ Installation & Usage

### Clone the repository

```bash
git clone https://github.com/yourusername/stock-price-lstm.git
cd stock-price-lstm

-> Install dependencies
pip install -r requirements.txt

📌 Future Enhancements
Integrate more stock symbols dynamically

Add ARIMA model or Transformer-based models for comparison

Build a Streamlit or Flask dashboard for interactive live predictions

🔗 References
Yahoo Finance API via yfinance

LSTM for Time-Series Forecasting

Keras Documentation
  
