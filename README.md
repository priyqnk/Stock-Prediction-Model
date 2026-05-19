# Stock Prediction Model

An interactive **Streamlit** app that forecasts stock prices using Meta's **Prophet** time-series model. Pulls historical data from Yahoo Finance via `yfinance` and visualizes predictions with Plotly.

## Features

- **Ticker selection** — Popular symbols including GOOG, AAPL, MSFT, and more
- **Historical data** — Live price history fetched with `yfinance`
- **Forecasting** — Prophet-based predictions up to three years ahead
- **Interactive charts** — Plotly visualizations for history and forecast bands
- **Model metrics** — MAPE and RMSE on held-out data

## Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Python 3.x |
| UI | Streamlit |
| Forecasting | Prophet |
| Data | yfinance, pandas, NumPy |
| Charts | Plotly |
| Metrics | scikit-learn |

## Project Structure

```
Stock-Prediction-Model/
├── stock_predictor.py      # Main Streamlit application
├── requirements.txt
├── Procfile                # Deployment process file
├── setup.sh                # Environment setup for hosting
├── runtime.txt             # Python version pin
└── README.md
```

## Getting Started

### Prerequisites

- Python 3.8+ (see `runtime.txt` for the pinned version used in deployment)

### Installation

```bash
git clone https://github.com/priyqnk/Stock-Prediction-Model.git
cd Stock-Prediction-Model

pip install -r requirements.txt
```

### Usage

```bash
streamlit run stock_predictor.py
```

Open the URL shown in the terminal (typically `http://localhost:8501`), pick a stock, and generate a forecast.

## Deployment

The repo includes files for cloud hosting (e.g. Streamlit Community Cloud or Heroku):

| File | Purpose |
|------|---------|
| `Procfile` | Start command for the host platform |
| `setup.sh` | Shell setup for deployment environments |
| `runtime.txt` | Python version specification |

## Disclaimer

This project is for **educational and demonstration purposes only**. Forecasts are not financial advice. Past performance does not guarantee future results.
