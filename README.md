# 📈 Stock Prediction App using Machine Learning & Flask

> Predict future stock prices with LSTM deep learning models — beautiful modern UI, interactive charts, and multiple features to analyze!

---

## 🌟 Features

- 📊 Predict stock prices (Close, Open, High, Low, Volume)
- 🏢 Select among multiple companies (AAPL, GOOG, MSFT, AMZN, FB)
- 🤖 Trained LSTM model for accurate sequential prediction
- 📈 Beautiful Plotly.js charts (Actual vs Predicted visualization)
- 🎨 Modern, responsive UI built with HTML, CSS, and Flask
- ⚡ Fast API backend for real-time predictions
- 🔥 Scalable for more companies and more timeframes
- 🛠️ Easy to extend with your own models and datasets

---

## 🚀 Project Structure

```
📁 Stock-Prediction-ML-Project
│
├── app.py                # Main Flask Application
├── predict.py            # Model training & prediction logic
├── lstm_stock_model.h5    # Saved LSTM model file
├── all_stocks_5yr.csv     # Dataset (5 years of stock data)
│
├── templates/
│   ├── index.html         # Home page (modern form to select options)
│   └── result.html        # Result page (plots and prediction)
│
├── static/
│   └── style.css          # Custom CSS styles
│
└── README.md              # Project documentation
```

---

## 📦 Installation

1. **Clone the repo:**
   ```bash
   git clone https://github.com/yourusername/Stock-Prediction-ML-Project.git
   cd Stock-Prediction-ML-Project
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

   _If `requirements.txt` is not created, install manually:_
   ```bash
   pip install flask tensorflow keras scikit-learn pandas plotly
   ```

3. **Run the app:**
   ```bash
   python app.py
   ```

4. **Open browser:**  
   Navigate to `http://127.0.0.1:5000/`

---

## 🧠 How it Works

- **Model**: An LSTM (Long Short-Term Memory) neural network trained on 5 years of stock data (`all_stocks_5yr.csv`).
- **Training**: 
  - 60 previous days → predict the next stock price.
  - Features like `close`, `open`, `high`, `low`, and `volume`.
- **Prediction**:
  - The user selects a **company** and a **feature** (e.g., Close Price).
  - The backend (`predict.py`) dynamically processes data and gives predicted values.
- **Visualization**:
  - Plotly charts show **Actual vs Predicted** trends in a modern graph.

---

## 🛠️ Technologies Used

- **Python 3.12+**
- **Flask** (Web Framework)
- **TensorFlow/Keras** (Deep Learning)
- **Plotly.js** (Interactive Graphs)
- **Pandas & Numpy** (Data Handling)
- **HTML5, CSS3** (Frontend)

---

## 📈 Sample Preview

| Home Page | Prediction Chart |
|:---:|:---:|
| ![Home Page Screenshot](screenshots/home.png) | ![Chart Screenshot](screenshots/chart.png) |

---

## 🚀 Future Enhancements

- Add more companies dynamically 📈
- Allow users to choose prediction periods (7 days, 30 days, etc.)
- Add **technical indicators** (SMA, EMA, MACD) to graphs 📊
- Integrate email alerts for target stock prices 📧
- Deploy app to cloud (Render / AWS / Azure) ☁️
- Add user login/signup with personalized portfolios 🧑‍💻
- Live stock updates with APIs like Yahoo Finance 🛰️
- Dashboard analytics for companies 🖥️

---

## 🤝 Contributing

Contributions are welcome!  
Please open an Issue or a Pull Request if you'd like to collaborate.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 🌟 Acknowledgements

- Kaggle Dataset: [5 Years Stock Prices Dataset](https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs)
- TensorFlow/Keras for deep learning models
- Plotly for beautiful graph visualizations

---

# 🔥 Let's Predict the Future... One Stock at a Time! 🚀
