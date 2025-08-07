# Customer Churn Prediction

This project predicts whether a bank customer is likely to churn (leave the bank) using a trained TensorFlow deep learning model. It processes structured input data (demographics and financial info), applies preprocessing (scaling, encoding), and outputs a churn probability.

🔗 **Live App**: [https://churn-predictor-090909.streamlit.app](https://churn-predictor-090909.streamlit.app)

---

## 🖥️ About the App

This web application takes user input such as Credit Score, Geography, Gender, Age, Tenure, Balance, etc., and predicts whether the customer will churn. It's designed for quick testing, experimentation, or demonstration of predictive analytics in banking.

---

## ✅ Features

- Simple and fast user interface (built with Streamlit)
- Real-time predictions with probability output
- Integrated with trained Keras model
- Preprocessing includes OneHotEncoding, LabelEncoding, and Feature Scaling

## 🧠 How It Works

1. User provides customer data via the Streamlit form.
2. The app:
   - Loads the trained `model.h5`
   - Applies `LabelEncoder`, `OneHotEncoder`, and `StandardScaler` using pre-saved `.pkl` files
   - Feeds processed data to the model
   - Outputs probability and churn prediction
3. Result is displayed as:
   - `The customer is likely to churn`
   - or `The customer is not likely to churn`

---

## ⚙️ Technologies Used

- Python
- TensorFlow / Keras
- Streamlit
- scikit-learn
- NumPy / Pandas
- Pickle

---

## 🚀 Run Locally

Clone the repository and install dependencies:

```bash
git clone https://github.com/your-username/churn-predictor.git
cd churn-predictor
pip install -r requirements.txt

Run the app
streamlit run app.py
