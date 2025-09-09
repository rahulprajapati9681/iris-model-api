🌸 Iris Species Prediction API – Explained

This repository is all about taking a machine learning model (Logistic Regression trained on the famous Iris dataset) and turning it into something the world can actually use:
👉 A REST API that predicts the species of an Iris flower.

Instead of keeping your ML model just in Jupyter Notebook, here you’re serving it as a live service so anyone can send data and get predictions instantly.

🔑 What’s happening here?

Model Training (Already Done)

The Iris dataset (Sepal Length, Sepal Width, Petal Length, Petal Width) is used.

A Logistic Regression model is trained.

That trained model is saved as a .pkl file (iris_LogesticRegression_model.pkl).

Flask API (model_api.py)

The saved model is loaded inside Flask.

An endpoint /predict is created that accepts JSON input:

{
  "features": [5.1, 3.5, 1.4, 0.2]
}


The API processes the input and returns the prediction, e.g. "Iris-setosa".

Frontend (web/)

A simple webpage with a form where users enter flower measurements.

When the form is submitted, it calls the API and shows the prediction in real time.

Deployment Support

requirements.txt → lists dependencies (Flask, joblib, etc.).

Procfile → tells platforms like Heroku/Railway how to run the API.

ngrok → helps expose your local API to the internet for quick demos.

✨ Why this repo is cool?

It’s a complete ML deployment workflow in one place:

ML Model ✅

API Service ✅

Frontend ✅

Deployment Ready ✅

Shows how real-world apps work:

User → sends data through a form or API call.

Server → processes it with ML model.

User → gets the prediction back instantly.

Beginner friendly 💡 → Anyone can clone, run, and test it with Postman or the web UI.

🚀 Big Picture

This repo teaches you:

How to wrap ML models into APIs

How to test APIs with Postman

How to expose APIs with ngrok for public use

How to connect frontend ↔ backend smoothly

How to prepare code for deployment on cloud platforms

💡 In short:
This repo is a mini production-grade ML project where machine learning meets software engineering. It shows how to go from “I trained a model” → “I built an app people can actually use.”
