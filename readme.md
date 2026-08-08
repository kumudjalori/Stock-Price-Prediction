# 📈 Stock Price Prediction Using LSTM

This project uses **Long Short-Term Memory (LSTM)** neural networks to predict future stock prices based on historical data. The model is trained on Google stock price data from **2012 to 2016** and predicts stock prices for **January 2017**.

---

## 📂 Dataset

- Dataset used: **Google Stock Price**
- Features used: `Open` price
- Training data: 2012–2016
- Test data: January 2017

---

## 🧠 Model Architecture

- Model: LSTM (Long Short-Term Memory)
- Input: Past 60 days of stock prices
- Output: Predicted next day's stock price
- Layers:
  - LSTM layers
  - Dropout for regularization
  - Dense output layer
- Framework: TensorFlow / Keras

---

## 📌 Steps Involved

1. **Data Preprocessing**
   - Feature scaling using `MinMaxScaler`
   - Creating time-series input windows (60 timesteps)
   - Reshaping for LSTM input: `(samples, timesteps, features)`

2. **Model Building**
   - Built using Keras Sequential API
   - Trained on historical data to minimize MSE loss

3. **Prediction**
   - Predicted stock prices for January 2017
   - Compared against real stock prices

4. **Evaluation**
   - RMSE and MAE metrics calculated
   - Visual comparison via matplotlib graphs
   - Achieved a prediction error of just 1.86% RMSE
---

## 📊 Results

- ✅ Smooth prediction curve closely following real prices
- ✅ Good generalization on unseen test data

---
