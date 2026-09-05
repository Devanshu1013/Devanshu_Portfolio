# Energy Forecasting

🔗 **Original Repository:** [github.com/Devanshu1013/Energy-Forecasting](https://github.com/Devanshu1013/Energy-Forecasting)

[← Back to portfolio](../README.md)

---

A comparative study of deep learning architectures for multivariate energy time-series forecasting. Uses 8 hours of historical sensor readings to predict the next energy consumption reading, benchmarking four different model families.

**Highlights:**
- Compares LSTM, TCN, Transformer, and LSTNet architectures on the same forecasting task
- Trained on the UCI Appliances Energy Prediction dataset (~19,700 rows, 10-minute intervals)
- Includes multi-horizon forecasting and sequence-length ablation experiments
- Chronological train/val/test split to avoid data leakage

**Tech stack:** `Python` `PyTorch` `LSTM` `TCN` `Transformer` `LSTNet`

![Model Comparison — MAE and RMSE](../assets/energy-forecasting-preview.png)

---

[← Back to portfolio](../README.md) &nbsp;|&nbsp; [🔗 View on GitHub](https://github.com/Devanshu1013/Energy-Forecasting)
