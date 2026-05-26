# Student Performance Prediction - Logistic Regression Model

A machine learning project that predicts a student performance category (Low, Medium, High) using logistic regression.

## Project overview

This project mirrors the linear regression project structure but uses a classification model. It includes:
- A Jupyter notebook for training and evaluation
- A Streamlit app for interactive predictions
- Model and metadata artifacts for deployment

## Dataset

The project uses student_performance_dataset.csv with the target column:
- performance_category (Low, Medium, High)

The model is trained with these input features:
- age
- gender
- city_type
- study_hours_per_day
- sleep_hours
- stress_level
- motivation_level
- focus_score
- attendance_percentage
- assignment_completion_rate

## Project structure

logistic/
- logistic_reg.ipynb
- app.py
- requirements.txt
- readme.md
- student_performance_dataset.csv
- logistic_regression_model.pkl
- model_metadata.json

## How to run

1. Install dependencies:

pip install -r requirements.txt

2. Train and export model (if needed):

Open logistic_reg.ipynb and run all cells.

3. Run Streamlit app:

streamlit run app.py

## Notes

- The app applies the same one-hot encoding pattern used in training.
- Feature alignment is handled with metadata to keep prediction columns consistent.
