# Flask-based Machine Learning Prediction Application
This project demonstrates a Flask web application for predicting outcomes based on user inputs using a trained machine learning model. The application takes data such as demographic details and test scores, preprocesses it, and predicts the outcome using a pre-trained model.




### Features
Interactive Web Interface: Users can input their data through a simple and user-friendly form.
Dynamic Data Prediction: The application processes user inputs and provides predictions in real-time.
Scalable Design: Easily extendable for other datasets and machine learning models.


### Requirements
To install the required packages, run:
pip install -r requirements.txt


### Input Data
The application accepts the following inputs:

Gender: Male/Female
Race/Ethnicity: Categorical variable
Parental Level of Education: Categorical variable
Lunch: Type of lunch (standard or free/reduced)
Test Preparation Course: Completed or not
Reading Score: Integer value
Writing Score: Integer value


### Output
The model predicts and displays the outcome based on the input data provided by the user. The results are shown on the home.html page.

### Directory Structure
├── artifacts/                    # Directory for generated artifacts

│   ├── data.csv                  # Raw dataset

│   ├── test.csv                  # Test dataset

│   ├── train.csv                 # Training dataset

├── logs/                         # Directory for log files

├── src/

│   ├── mlproject/

│       ├── components/           # Core ML components

│       │   ├── data_ingestion.py # Handles data ingestion

│       │   ├── data_transformation.py # Data preprocessing

│       │   ├── model_monitoring.py # Monitoring model performance

│       │   ├── model_trainer.py  # Model training logic

│       ├── pipelines/            # Pipelines for prediction and other tasks

│       │   ├── __init__.py

│       │   ├── prediction_pipeline.py # Pipeline for making predictions

│       ├── __init__.py

│       ├── exception.py          # Custom exception handling

│       ├── logger.py             # Logging utility

│       ├── utils.py              # Utility functions

├── templates/

│   ├── home.html                 # Main input form page

│   ├── index.html                # Landing page

├── venv/                         # Virtual environment directory

├── app.py                        # Flask application entry point

├── README.md                     # Project documentation

├── requirements.txt              # Python dependencies

├── setup.py                      # Installation setup

└── template.py                   # Template script for custom utilities
