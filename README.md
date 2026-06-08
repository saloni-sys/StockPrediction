# Stock Trend Prediction Using LSTM

## Overview

This project is a Stock Trend Prediction System built using Long Short-Term Memory (LSTM) networks. The model analyzes historical stock closing prices and learns temporal patterns to predict future stock price trends.

A Streamlit web application is integrated with the trained model, allowing users to enter a stock ticker symbol and visualize historical trends along with predicted stock prices.

---

## Features

* Fetches historical stock data using Yahoo Finance
* Visualizes stock closing prices over time
* Displays 100-day and 200-day Moving Averages
* Uses LSTM (Long Short-Term Memory) neural networks for time-series prediction
* Predicts future stock price trends based on historical data
* Interactive Streamlit web application
* Supports different stock ticker symbols

---

## Project Workflow

### 1. Data Collection

Historical stock market data is collected using the Yahoo Finance API through the `yfinance` library.

### 2. Data Preprocessing

* Extracts stock closing prices
* Splits data into training and testing sets
* Normalizes data using MinMaxScaler
* Creates 100-day sequences for LSTM training

### 3. Model Development

An LSTM-based deep learning model is trained on historical stock price data to learn temporal dependencies and trends.

### 4. Prediction

The trained model predicts stock prices using the previous 100 days of stock data.

### 5. Visualization

The application displays:

* Closing Price vs Time
* Closing Price with 100-Day Moving Average
* Closing Price with 100-Day and 200-Day Moving Averages
* Original vs Predicted Stock Prices

---

## Technologies Used

### Programming Language

* Python

### Libraries

* NumPy
* Pandas
* Matplotlib
* TensorFlow / Keras
* Scikit-learn
* Yahoo Finance (yfinance)
* Streamlit

---

## Model Architecture

The project uses a stacked LSTM architecture consisting of:

* Multiple LSTM layers
* Dropout layers for regularization
* Dense output layer for price prediction

The model learns sequential patterns from stock closing prices and predicts future trends.

---

## Dataset

Data Source:

* Yahoo Finance

Stock Example:

* Apple Inc. (AAPL)

Time Period:

* 2010 – 2019

Feature Used:

* Closing Price

---

## Running the Project

### Clone Repository

```bash
git clone <https://github.com/saloni-sys/StockPrediction>
cd StockPrediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Streamlit App

```bash
streamlit run app.py
```

---

## Results

The model successfully captures the overall trend of stock movements and generates predictions that closely follow historical price patterns.

While the model can identify general market trends, stock prices are influenced by many external factors such as:

* Market sentiment
* Financial news
* Economic indicators
* Company fundamentals

Therefore, predictions should be considered educational and experimental rather than financial advice.



## Learning Outcomes

Through this project, I learned:

* Time-series forecasting fundamentals
* Data preprocessing and normalization
* Sequence generation for LSTM networks
* Deep learning model training using TensorFlow/Keras
* Model evaluation and visualization
* Streamlit application development
* Debugging machine learning pipelines and scaling issues

---

## Disclaimer

This project is intended for educational and learning purposes only. It should not be used as financial or investment advice.

