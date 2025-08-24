# 📈 Google Stock Price Prediction by using LSTM

This project uses **Long Short-Term Memory (LSTM)**, a type of Recurrent Neural Network (RNN), to predict future stock prices of **Google (GOOGLE)** based on historical data. LSTM models are effective for time series forecasting due to their ability to learn long-term dependencies        
                 
---               
## Author : Shashank Pandey                     
      
          
## 📊 Project Overview     

Stock price prediction is a challenging and fascinating task. In this project, we use an LSTM-based deep learning model to predict Google's stock prices using its historical data.

The model is trained on past stock prices and aims to predict the stock's future closing prices. It provides a basic but powerful demonstration of how deep learning can be used in financial forecasting.

---
 
## 🧾 Dataset

- Source: Yahoo Finance (GOOGL stock)
- Features Used:
  - `Open`
  - `High`
  - `Low`
  - `Close`
  - `Volume`
- The dataset is split into training and testing sets.
- Data is scaled using MinMaxScaler for better model performance.

---

## 🔧 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib / Seaborn
- TensorFlow / Keras
- Scikit-learn

---

## 🚀 How to Run the Project

1. **Clone the Repository**

     ```bash
   git clone https://github.com/webvokess/Google-Stock-Price-Prediction-using-LSTM.git
   cd Google-Stock-Price-Prediction-using-LSTM

2. **Install Required Libraries**
     ```bash
     pip install -r requirements.txt
     
3. **Run the Notebook**
     ```bash
     pip install numpy pandas matplotlib seaborn scikit-learn tensorflow

## 📈 Model Architecture

The LSTM model consists of the following layers:

- **Input Layer:** Preprocessed stock price sequences
- **LSTM Layer 1:** Captures temporal patterns in the data
- **LSTM Layer 2 (optional):** Stacked LSTM to deepen learning
- **Dropout Layers:** Prevent overfitting
- **Dense Layer:** Single output neuron to predict the next closing price

**Model Configuration:**

- **Loss Function:** Mean Squared Error (MSE)
- **Optimizer:** Adam
- **Activation Functions:** `tanh` in LSTM, linear in output

---

## 📌 Results

- The model was able to **predict Google's stock closing prices** with a trend closely following actual values.
- Visualization typically shows:
  - **Blue Line:** Real historical prices
  - **Red/Orange Line:** Predicted prices

### Key Takeaways:
- LSTM effectively learns temporal dependencies in stock price data.
- Predictions help in understanding potential future price movements.

---

## 📉 Limitations

- The model **does not include** external factors such as news, market sentiment, or economic indicators.
- It uses only **historical price data**, which limits real-world forecasting accuracy.
- Real-time or frequent retraining is required for production use.
- No technical indicators (e.g., RSI, MACD) are included — adding these could improve performance.

