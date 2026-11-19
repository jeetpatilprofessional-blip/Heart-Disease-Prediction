# Heart Disease Prediction | Machine Learning

## Overview
A learning project that builds a binary classification model to estimate whether a record in the supplied dataset is associated with heart disease. A Streamlit interface provides an interactive way to explore the model's output.

> **Educational project only:** This model is not clinically validated and must not be used for diagnosis, treatment, or medical decision-making.

## Features
- Interactive Streamlit interface
- Data processing and model-based prediction
- Python notebook for exploration/model development
- Scikit-learn model artifact

## Technology
Python • Pandas • NumPy • Scikit-learn • Streamlit • Jupyter Notebook

## Dataset
The dataset includes commonly used features such as age, sex, chest-pain type, resting blood pressure, cholesterol, fasting blood sugar, maximum heart rate, exercise-related angina, ST depression, vessel count, thalassemia and a target label.

## Files
- `app.py` — Streamlit interface
- `heart_disease.ipynb` — notebook
- `heart.csv` — dataset
- `heart-disease-model.pkl` — saved model
- `requirements.txt` — dependencies

## Run Locally
```bash
git clone https://github.com/jeetpatilprofessional-blip/Heart-Disease-Prediction.git
cd Heart-Disease-Prediction
pip install -r requirements.txt
streamlit run app.py
```

## Evaluation
Please refer to the notebook for the actual training and evaluation workflow. Model metrics should be reported only after verifying the notebook outputs; this README does not claim clinical performance.

## Limitations
Dataset bias, data quality, preprocessing choices, model calibration and external validation all affect results. The output is a machine-learning estimate and is not a medical diagnosis.
