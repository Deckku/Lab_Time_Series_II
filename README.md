# Lab_Time_Series_II
# Time Series Sales Forecasting with Recurrent Neural Networks

## What Is a Time Series?

A **time series** is a sequence of data points indexed or listed in chronological order. Time-series data are often collected at regular time intervals (daily, monthly, yearly), but can also be irregular. They appear in many fields such as finance (stock prices), meteorology (temperature), economics (GDP), and of course, product sales.

Time-series analysis aims to understand the underlying patterns that generate these sequences and to predict their future values. Key characteristics include trends (long-term increases or decreases), seasonality (recurring patterns at fixed intervals), and cycles (fluctuations without a fixed period).

## Our Project: Sales Prediction

In this project, we focused on sales forecasting. We used historical sales data to train several neural-network models to predict future sales.

### Key Steps of the Project:

1. **Data Collection and Reduction:**  
   We started with a large sales dataset (M5 Forecasting Accuracy competition). For performance and clarity, we reduced it to a more manageable subset of items and a shorter time window (the first 180 days of sales for selected items).

2. **Data Preparation:**  
   The sales data were transformed into a format suitable for time-series models. This involved building sequences of past observations (`lookback`) to predict future values (`forecast horizon`). The data were also normalized to improve neural-network performance.

3. **Model Construction and Training:**  
   We explored several neural-network architectures commonly used for time-series forecasting:
   * **Simple RNN (Recurrent Neural Network):** Designed to process sequential data.
   * **LSTM (Long Short-Term Memory):** An improved RNN capable of capturing long-range dependencies.
   * **GRU (Gated Recurrent Unit):** Similar to LSTM but with a simplified structure, often faster while offering comparable performance.
   * **MLP (Multilayer Perceptron):** A classic feedforward neural network used here as a baseline to compare its behavior on sequential data.

4. **Performance Evaluation:**  
   Each model was trained and evaluated on its ability to predict future sales. We used metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), and Mean Absolute Percentage Error (MAPE) to assess prediction accuracy.

## Credits
* Author: Azami Hassani Adnane.
* Supervisor: Prof. Masrour Tawfik.
This project demonstrates the practical use of recurrent neural networks for time-series forecasting in a sales context, highlighting different approaches and their comparative performance.
