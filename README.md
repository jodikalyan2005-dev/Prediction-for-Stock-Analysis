💰 **Stock Price Prediction using Time Series Analysis**
This project demonstrates a fundamental approach to time series forecasting by predicting the daily closing price of a stock using its historical data.

🎯 **Project Goal**
Perform time series analysis on historical stock data (stocks.csv).

**Develop a predictive model to forecast future closing prices.**

Evaluate the model's performance using standard regression metrics.

🛠️ Tools and Technologies
Category	Tools Used
Programming	Python
Data Handling	pandas (Data manipulation)
Modeling	scikit-learn (Linear Regression)
Visualization	matplotlib
Numerical Computing	NumPy

Export to Sheets
🧠 **Methodology (How it was done)**
Data Loading and Preprocessing: Loaded the stocks.csv file, converting the Date column to the datetime format and setting it as the index.

_Feature Engineering (Lagging): Transformed the time series problem into a supervised learning problem by creating lagged features. The Close price of the current day was predicted using the Close prices of the preceding 7 days.

Data Splitting: The dataset was split into training and testing sets, reserving the last ≈20% of the chronological data for testing to simulate a real-world forecasting scenario.

Model Training: A Linear Regression model was trained on the lagged features to learn the linear relationship between past prices and the current price.

Evaluation: Performance was assessed using RMSE and MAE to quantify the magnitude of prediction errors.

🚀 Future Enhancements
Advanced Models: Implement specialized time series models like ARIMA/SARIMA, or deep learning models like LSTMs (Long Short-Term Memory), which are better suited for capturing stock market non-linearity.

![Code_Generated_Image (1)](https://github.com/user-attachments/assets/2c428e8b-bed2-498b-86d0-96c148535f23)
**
Additional Features:** Incorporate technical indicators (e.g., Moving Averages, RSI, MACD) as features to improve predictive accuracy.

**Hyperparameter Tuning:** Optimize the current model by testing different lag lengths (e.g., 3,5,10 days).
