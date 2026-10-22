# HealthEdge – ML-Based Diabetes Prediction System

## About the Project

HealthEdge is a machine learning-based web application developed using Python and Django to predict the risk of Type 2 diabetes from patient health data. It uses a Random Forest classification model to generate predictions based on relevant medical parameters.

The application is designed to support healthcare professionals in preliminary diabetes risk assessment by providing prediction results through a user-friendly interface.

## Key Features

- **Machine Learning Prediction:** Uses a trained Random Forest classification model.
- **User Authentication:** Provides login and registration functionality for authorized users.
- **Patient Information Entry:** Allows users to enter relevant patient details and health parameters.
- **Prediction Results:** Displays the model's prediction to support preliminary risk assessment.
- **Prediction History:** Allows logged-in users to review previous patient predictions.
- **User-Friendly Interface:** Provides a structured interface for accessing the application's features.

## Technologies Used

- **Programming Language:** Python
- **Web Framework:** Django
- **Machine Learning:** Scikit-learn
- **ML Algorithm:** Random Forest Classifier
- **Frontend:** HTML, CSS
- **Database:** Django-supported database, depending on project configuration
- **Model Storage:** Pickle (`.pkl`)

## Machine Learning Workflow

1. Data collection
2. Data cleaning and preprocessing
3. Feature preparation
4. Training the Random Forest classification model
5. Model evaluation
6. Integration of the trained model into Django
7. Prediction generation through the web application

## Project Structure

The application contains Django project files and separate applications for user management and diabetes prediction.

- `usermod/` – User registration and login functionality
- `predictionmod/` – Diabetes prediction and related application functionality
- `templates/` – HTML templates
- `static/` – CSS and other static assets

## Installation and Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/aayisharazack/health-edge.git
   ```

2. Navigate to the project directory:

   ```bash
   cd health-edge
   ```

3. Create and activate a virtual environment:

   ```bash
   python -m venv env
   ```

   Windows:

   ```bash
   env\Scripts\activate
   ```

4. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Apply database migrations:

   ```bash
   python manage.py migrate
   ```

6. Start the development server:

   ```bash
   python manage.py runserver
   ```

7. Open `http://127.0.0.1:8000/` in your browser.


## Limitations

- Predictions depend on the quality and characteristics of the training data.
- Model outputs may not generalize to every patient population.
- Predictions are not a substitute for professional medical diagnosis or clinical evaluation.

## Future Enhancements

- Improve model evaluation using additional datasets and validation techniques.
- Enhance prediction reports and data visualization.
- Introduce prescription management and patient access features.
- Explore additional machine learning techniques and model improvements.

## Disclaimer

HealthEdge is an educational machine learning project. Its predictions should not be used as the sole basis for medical decisions and do not replace professional medical advice, diagnosis, or treatment.
