# Google-Stock-Price-Prediction-using-LSTM
Google Stock Price Prediction using Long Short-Term Memory (LSTM) is a deep learning-based approach to forecasting stock prices using historical data. LSTM is a type of recurrent neural network (RNN) that is well-suited for sequential data like stock prices.<br>
<b>Overview<b><br>
The goal of this project is to predict future stock prices of Google using past stock price data. Since stock prices follow time-series patterns, LSTMs can capture long-term dependencies and trends effectively.

<br><b>Steps Involved</b><br>
 Data Collection
Historical stock price data of Google (GOOGL) is collected from sources like Yahoo Finance, Alpha Vantage, or Kaggle.<br><br>
Data Preprocessing
Handling missing values.
Feature scaling using MinMaxScaler to normalize the data.
Creating sequences of past stock prices as input and future stock prices as output.
Building the LSTM Model

The LSTM model consists of multiple layers:
Input Layer
LSTM Layers (to capture dependencies in stock price movements)
Dense (Fully Connected) Layers for final prediction
Loss function: Mean Squared Error (MSE)
Optimizer: Adam
Training the Model

The model is trained using historical stock data.
A portion of the dataset is used for training and another portion for validation/testing.
Making Predictions

The trained LSTM model predicts stock prices for the next time steps.
Results are compared with actual stock prices.
Visualization

Stock price predictions vs. actual prices are plotted for better analysis.
Key Features of LSTM in Stock Prediction
Captures long-term dependencies in time-series data.
Prevents vanishing gradient problem, which occurs in traditional RNNs.
Can model complex stock price movements.
Challenges
Stock prices are influenced by many external factors like news, economic events, and investor sentiment, which are not captured by LSTM alone.
Hyperparameter tuning is essential for improving accuracy.
