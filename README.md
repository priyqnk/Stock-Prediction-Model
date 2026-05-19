# Stock Forecast App

An interactive Streamlit application that leverages historical stock data to forecast future prices using Meta's **Prophet** model.

## Features

- **Interactive Selection**: Choose from popular stocks like GOOG, AAPL, MSFT, and more.
- **Historical Analysis**: Fetches real-time historical data using `yfinance`.
- **Advanced Forecasting**: Predicts stock price trends for up to 3 years into the future.
- **Interactive Visualizations**: High-quality charts powered by `Plotly`.
- **Performance Metrics**: Calculates MAPE (Mean Absolute Percentage Error) and RMSE (Root Mean Square Error) for model evaluation.

## Installation

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd stock-prediction-model
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

To run the Streamlit app locally:
```bash
streamlit run stock_predictor.py
```

## Deployment

The project is ready for deployment (e.g., on Heroku or Streamlit Cloud) with the following files:
- `Procfile`: Command for deployment.
- `setup.sh`: Environment setup script.
- `runtime.txt`: Specifies Python version.

## Technologies Used

- **Streamlit**: For the web interface.
- **Facebook Prophet**: For time-series forecasting.
- **yfinance**: To fetch stock data from Yahoo Finance.
- **Plotly**: For interactive charts.
- **Pandas/Numpy**: For data manipulation.
- **Scikit-learn**: For evaluation metrics.
