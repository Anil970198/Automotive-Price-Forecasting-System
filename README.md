# Automotive-Price-Forecasting-System

This project is a Flask-based web application that predicts the resale price of a car based on various input features. The application uses a pre-trained Random Forest Regressor model to make predictions. The model is trained on a dataset of car details and integrates user inputs through a web form to provide predictions.

Project Structure

app.py: The main Python file for running the Flask application.

rfrm.pkl: The serialized Random Forest Regressor model used for prediction.

templates/index.html: The HTML template for the web interface.

my_dataset.csv: The dataset used for training the model.

Features

User-Friendly Interface: Input car details such as year of purchase, price, mileage, owner type, and fuel type through a web form.

Data Preprocessing: Automatically preprocesses input data to make it compatible with the model.

Prediction: Provides the resale price of the car or suggests that the car cannot be sold if the price is negative.

Machine Learning Pipeline: Utilizes a Random Forest Regressor trained on relevant car data.

Installation and Setup

Clone the repository:

git clone <repository_url>
cd <repository_folder>

Install dependencies:

pip install -r requirements.txt

Place the trained model file (rfrm.pkl) in the project directory.

Run the application:

python app.py

Access the application at http://127.0.0.1:5000.

Dataset

The model was trained using a dataset containing the following columns:

Year: Year of manufacture.

Selling_Price: Selling price of the car (target variable).

Present_Price: Current ex-showroom price.

Kms_Driven: Total kilometers driven by the car.

Fuel_Type: Type of fuel (Petrol/Diesel).

Seller_Type: Whether the seller is a dealer or an individual.

Transmission: Type of transmission (Manual/Automatic).

Owner: Number of previous owners.

Model Training

Data Cleaning and Feature Engineering:

Removed missing values.

Created new features like no_year (age of the car).

One-hot encoded categorical variables.

Exploratory Data Analysis (EDA):

Visualized correlations between features using heatmaps.

Identified important features using ExtraTreesRegressor.

Model Selection and Hyperparameter Tuning:

Trained a RandomForestRegressor.

Tuned hyperparameters using RandomizedSearchCV.

Performance Metrics:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Key Python Libraries Used

Flask: Web application framework.

NumPy: Numerical computations.

Pandas: Data manipulation.

Scikit-learn: Machine learning.

Seaborn and Matplotlib: Data visualization.

Pickle: Model serialization.

How It Works

User Input:

The user provides car details through a web form.

Preprocessing:

Converts categorical inputs to numerical values.

Calculates derived features such as the age of the car.

Prediction:

Passes the preprocessed inputs to the trained model.

Returns the predicted price or an error message if the car cannot be sold.

Output:

Displays the result on the same webpage.

Example Usage

Enter details such as year of purchase, present price, kilometers driven, and fuel type.

Click the "Predict" button.

View the predicted resale price or an appropriate message.

Future Improvements

Add more user-friendly error handling and validation for form inputs.

Enhance the model with additional features or a larger dataset.

Deploy the application to a cloud service (e.g., AWS, Heroku) for public access.

Include visualizations of the prediction results.

Contributors

[Your Name] (your_email@example.com)

Feel free to fork, contribute, and submit issues for improvement!


