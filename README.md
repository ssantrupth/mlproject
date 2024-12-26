# Student Maths Marks Prediction

This project aims to predict students' math scores based on their demographics and academic background using a machine learning model. It leverages Flask to create a web-based interface where users can input relevant information and get predictions.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Setup Instructions](#setup-instructions)
5. [Running the Application](#running-the-application)
6. [Project Workflow](#project-workflow)
7. [Usage](#usage)
8. [Future Improvements](#future-improvements)

---

## Project Overview

This project uses demographic and academic information about students to predict their math scores. It incorporates machine learning models trained on historical data and serves predictions via a web application. The project is useful for understanding the factors affecting students' academic performance and assisting educators in identifying students who may need support.

### Input Features:
- **Gender**: Gender of the student (e.g., Male, Female).
- **Race/Ethnicity**: Group to which the student belongs.
- **Parental Level of Education**: Highest level of education attained by the parents.
- **Lunch**: Type of lunch the student receives (e.g., Standard or Free/Reduced).
- **Test Preparation Course**: Whether the student completed a test preparation course.
- **Reading Score**: Reading score of the student.
- **Writing Score**: Writing score of the student.

### Output:
- Predicted Math Score

---

## Features

- Train machine learning models to predict math scores.
- Hyperparameter tuning using GridSearchCV.
- RESTful web interface using Flask.
- Save and load the best-trained model for predictions.
- Modular code structure for scalability.

---

## Technologies Used

- **Programming Language**: Python (3.9)
- **Libraries**:
  - Flask
  - Scikit-learn
  - CatBoost
  - XGBoost
  - Pandas
  - NumPy
  - Joblib
  - Logging
- **Tools**: SQLite (for database management), VS Code

---

## Setup Instructions

Follow the steps below to set up the project on macOS.

### Prerequisites
Ensure you have the following installed:
- Python (>=3.9)
- pip (Python package manager)
- Virtual environment support (`venv` or `virtualenv`)

### Step 1: Clone the Repository
```bash
# Clone the repository
git clone https://github.com/ssantrupth/mlproject.git
cd mlproject
```

### Step 2: Create a Virtual Environment
```bash
# Create a virtual environment
python3 -m venv project

# Activate the virtual environment
source project/bin/activate
```

### Step 3: Install Dependencies
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### Step 4: Verify Installation
Ensure all required packages are installed successfully.
```bash
pip list
```

---

## Running the Application

1. Activate the virtual environment (if not already activated):
    ```bash
    source project/bin/activate
    ```

2. Start the Flask server:
    ```bash
    python app.py
    ```

3. Open your browser and navigate to:
    ```
    http://127.0.0.1:4040
    ```

---

## Project Workflow

1. **Data Ingestion**:
   - Data is collected from CSV files and preprocessed.

2. **Model Training**:
   - Multiple regression models are trained and evaluated.
   - Hyperparameter tuning is performed using GridSearchCV.

3. **Model Evaluation**:
   - The best model is selected based on R2 score.

4. **Model Deployment**:
   - The best-performing model is saved and integrated into the Flask application for real-time predictions.

5. **Web Application**:
   - Users input student details to get predicted math scores.

---

## Usage

1. Open the Flask app in your browser.
2. Fill in the form with the following details:
   - Gender
   - Race/Ethnicity
   - Parental Level of Education
   - Lunch Type
   - Test Preparation Course
   - Reading Score out of 100
   - Writing Score out of 100
3. Submit the form to get the predicted math score.

---

## Future Improvements

- Enhance the UI/UX of the web application.
- Train the model with additional features for improved accuracy.
- Add support for other performance metrics.
- Deploy the application on cloud platforms (e.g., AWS, GCP, or Azure).
- Integrate database support for saving user inputs and predictions.

---

## Acknowledgments
This project is inspired by real-world educational datasets and aims to assist educators in analyzing student performance effectively.
