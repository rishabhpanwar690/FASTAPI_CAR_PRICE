# 🚗 Car Price Prediction System using FastAPI + Streamlit + Machine Learning

An end-to-end Machine Learning web application that predicts the selling price of used cars based on vehicle features.

The project uses a trained Random Forest Regression model served through a FastAPI backend and an interactive Streamlit frontend for users.

---

## 🌐 Live Demo

### 🚀 Streamlit Web App
```
https://fastapi-car-price-1.onrender.com/
```

### ⚡ FastAPI Backend (Swagger Docs)

```
https://car-prediction-lpfl.onrender.com/docs
```

---

# 📌 Project Overview

This project predicts used car prices using Machine Learning.

Users enter car information such as:

- Manufacturing year
- Kilometers driven
- Fuel type
- Seller type
- Transmission type
- Ownership history
- Mileage
- Engine capacity
- Maximum power
- Number of seats

The application processes these inputs and predicts the estimated selling price.

---

# 🏗️ System Architecture


User
 |
 v

Streamlit Frontend
 |
 | HTTP POST Request
 v

FastAPI Backend
 |
 v

Random Forest Regression Model
 |
 v

Predicted Car Price


---

# 🛠️ Tech Stack

## Machine Learning

- Python
- Pandas
- NumPy
- Scikit-Learn
- Random Forest Regressor
- Pickle

## Backend

- FastAPI
- Uvicorn
- Pydantic
- REST API

## Frontend

- Streamlit
- Requests Library

## Deployment

- Render
- GitHub

---

# 📂 Project Structure


FASTAPI_CAR_PRICE/

│

├── model/

│   └── car-price-api/

│       │

│       ├── main.py

│       ├── streamlit_app.py

│       ├── schema.py

│       ├── train.py

│       ├── random_forest_model.pkl

│       ├── feature_columns.pkl

│       ├── requirements.txt

│       └── README.md


---

# ⚙️ Installation & Setup

Clone the repository:

```bash
git clone https://github.com/rishabhpanwar690/FASTAPI_CAR_PRICE.git
```

Move into project:

```bash
cd FASTAPI_CAR_PRICE/model/car-price-api
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# 🚀 Run FastAPI Backend Locally


Start server:

```bash
uvicorn main:app --reload
```


Open:

```text
http://127.0.0.1:8000/docs
```

You will see FastAPI Swagger UI.

---

# 🎨 Run Streamlit Frontend


Start Streamlit:

```bash
streamlit run streamlit_app.py
```


Open browser:

```text
http://localhost:8501
```

---

# 🔥 API Endpoint


## Health Check

GET request:

```
/
```


Response:

```json
{
  "success": true,
  "message": "this is test route"
}
```

---

## Prediction Endpoint


POST:

```
/predict
```


Example Input:


```json
{
  "year": 2018,
  "km_driven": 50000,
  "fuel": "Petrol",
  "seller_type": "Individual",
  "transmission": "Manual",
  "owner": "First Owner",
  "mileage": 20.5,
  "engine": 1197,
  "max_power": 82,
  "seats": 5
}
```


Example Output:


```json
{
  "predicted_price": 650000
}
```

---

# 🤖 Machine Learning Workflow


1. Data Collection

2. Data Cleaning

3. Feature Engineering

4. Encoding Categorical Features

5. Model Training

6. Random Forest Regression

7. Model Serialization using Pickle

8. Deployment using FastAPI


---

# ⭐ Features


✔ Machine Learning Prediction

✔ REST API Backend

✔ Interactive Web Interface

✔ Automatic API Documentation

✔ Model Deployment

✔ Real-time Predictions

✔ Cloud Hosted Application


---

# 📈 Future Improvements


- Improve model accuracy
- Add more ML algorithms
- Add database storage
- User authentication
- Docker deployment
- CI/CD pipeline


---

# 👨‍💻 Author

**Rishabh Panwar**

GitHub:

```
https://github.com/rishabhpanwar690
```

---

# 📜 License

This project is open source and available for learning and development.

⭐ If you like this project, consider giving it a star!# FASTAPI_CAR_PRICE
