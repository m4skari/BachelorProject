# Markowitz Portfolio Optimization with Deep Learning-Based Stock Prediction

This repository contains my undergraduate thesis project at the University of Tehran, focused on portfolio optimization using Markowitz’s mean–variance model combined with deep learning-based stock price prediction.

📌 Project Overview

Financial markets are inherently uncertain, and predicting stock prices plays a crucial role in investment decisions. Traditional models like Markowitz’s mean–variance optimization rely heavily on historical data and may fail to adapt to dynamic market conditions.

In this project, I propose a hybrid framework that integrates:

Deep learning models (LSTM, BiLSTM, CNN-BiLSTM) for time series forecasting of stock prices.

Robust statistics (Huber’s M-estimator) for noise reduction in financial data.

Markowitz’s mean–variance optimization for constructing efficient portfolios based on predicted returns.

The results demonstrate that portfolios optimized with predicted returns significantly outperform equal-weighted portfolios, achieving higher Sharpe Ratios without substantially increasing risk


.

🔬 Methodology

Data Preprocessing

Collected S&P 500 historical closing prices (2013–2018).

Cleaned and normalized data using Huber’s M-estimator.

Generated 21-day rolling windows as input sequences.

Forecasting Models

LSTM – baseline model for long-term dependencies.

BiLSTM – bidirectional recurrent architecture for enhanced temporal learning.

CNN-BiLSTM – hybrid model combining local feature extraction with sequential dependency modeling.

Portfolio Construction

Selected top 10 stocks based on predicted returns.

Applied Markowitz’s mean–variance optimization to compute optimal weights.

Benchmarked against equal-weighted portfolios.

Evaluation Metrics

Prediction: MSE, MAE, SMAPE.

Portfolio: Mean Return, Standard Deviation, Sharpe Ratio.

📊 Results

CNN-BiLSTM outperformed other models in prediction accuracy.

Optimized portfolios achieved an average Sharpe Ratio ≈ 1.6 compared to 1.1 for equal-weighted portfolios.

In some intervals, the improvement was up to 2x higher Sharpe Ratio.

⚙️ Technologies & Tools

Python 3.10

Libraries: TensorFlow/Keras, NumPy, Pandas, Matplotlib, scikit-learn, cvxopt

📖 References

Markowitz Mean-Variance Portfolio Optimization with Predictive Stock Selection Using Machine Learning (MDPI, 2022)

Optimal Markowitz portfolio using returns forecasted with time series and machine learning models (Springer, 2025)

Return Prediction for Mean-Variance Portfolio Selection: Decision-Focused Learning (arXiv, 2025)

Hybrid Data-Driven and Deep Learning Based Portfolio Optimization (SCIRP, 2023)

Enhancing Black-Litterman Portfolio via Hybrid Forecasting (arXiv, 2025)

👤 Author

Mohammad Askari
B.Sc. in Electrical Engineering (Control)
University of Tehran
