# Automotive-Price-Forecasting-System
## Overview
This project is a Flask-based web application that predicts the resale price of a car based on various input features. The application uses a pre-trained Random Forest Regressor model to make predictions. The model is trained on a dataset of car details and integrates user inputs through a web form to provide predictions.
## Project Structure
* `app.py:`:Main Flask application handling routes and logic.
* `rfrm.pkl`:Pre-trained Random Forest Regressor model.
* `templates/`:Folder containing HTML file `index.html`
* `my_dataset.csv`: Dataset used for training the model.
## Installation and Setup
1. Clone the repository.

2. Install dependencies using `pip install -r requirements.txt.`

3. Run the Flask app with `python app.py.`

4. Access the application at `http://127.0.0.1:5000/` in your browser.

## Features
* User Inputs: Input car details like year, present price, kilometers driven, owner type, fuel type, seller type, and transmission type.

* Prediction: Displays the estimated selling price of the car.

* Model: Utilizes a Random Forest Regressor trained on a processed dataset.

## Prerequisites
```
certifi==2020.6.20
chardet==3.0.4
click==7.1.2
Flask==1.1.2
idna==2.10
itsdangerous==1.1.0
Jinja2==2.11.2
joblib==0.15.1
jsonify==0.5
MarkupSafe==1.1.1
numpy==1.19.0
requests==2.24.0
scikit-learn==0.23.1
scipy==1.5.0
sklearn==0.0
threadpoolctl==2.1.0
urllib3==1.25.9
Werkzeug==1.0.1
wincertstore==0.2
gunicorn
```

  # Overview of the dataset
  After meticulously treating the data correlation functions have been applied and this is the resulted table that shows the correlation among various features in the dataset![image](https://github.com/user-attachments/assets/8a3aba6b-89f0-4622-b55c-f0a252451cce)

# 
