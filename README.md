# Heart Disease Prediction App | Machine Learning

An educational machine learning project that uses a trained classification model to estimate a dataset-based heart-disease classification from user-entered health parameters. The model is presented through an interactive Streamlit application.

> **Disclaimer:** This project is an educational prototype, not a clinically validated medical tool. Its output must not be used for diagnosis, treatment, or medical decision-making. Consult a qualified healthcare professional for medical concerns.

## Application Preview

### Main interface
![Heart Disease Prediction App – main interface](Streamlit%20Interface.png)

### Input form and prediction action
![Heart Disease Prediction App – input form](Streamlit%20Interface%20(2).png)

## Features

- Interactive Streamlit interface with a two-column input form.
- Accepts demographic and health-related parameters, including age, gender, chest-pain type, resting blood pressure, cholesterol, fasting blood sugar, resting ECG, maximum heart rate, exercise-induced angina, ST depression, ST slope, major vessels, and thalassemia.
- Encodes categorical inputs and aligns them with the model's expected feature columns.
- Applies the saved scaler to numerical features before prediction.
- Displays a model classification message when the user selects **Predict Heart Disease Risk**.

## Machine Learning Workflow

1. Load the saved model and scaler from `heart-disease-model.pkl`.
2. Collect the 13 input attributes through the Streamlit form.
3. Convert the gender selection to the model's numeric representation.
4. Encode categorical fields using one-hot encoding.
5. Align the encoded input with the feature columns expected by the trained model.
6. Scale numerical features using the saved scaler.
7. Generate and display the model's predicted class.

The notebook `heart_disease.ipynb` contains the model-development workflow. Refer to it for the training and evaluation details. No performance metric is stated here because it should be taken directly from verified notebook results.

## Technology Stack

- Python
- Streamlit
- Pandas
- NumPy
- Scikit-learn
- Pickle
- Jupyter Notebook

## Repository Structure

```
Heart-Disease-Prediction/
├── app.py
├── heart_disease.ipynb
├── heart.csv
├── heart-disease-model.pkl
├── requirements.txt
├── Streamlit Interface.png
├── Streamlit Interface (2).png
└── README.md
```

## Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/jeetpatilprofessional-blip/Heart-Disease-Prediction.git
   cd Heart-Disease-Prediction
   ```

2. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Start the Streamlit application:

   ```bash
   streamlit run app.py
   ```

## Limitations

- The model is based on its training dataset and may not generalize to other populations or clinical settings.
- The application does not replace professional medical assessment.
- The model has not been established as clinically validated; predictions are for demonstration and learning only.

## Project Files

- `app.py` — Streamlit application and prediction flow.
- `heart_disease.ipynb` — notebook for model exploration and development.
- `heart.csv` — dataset used by the project.
- `heart-disease-model.pkl` — saved model and scaler.
- `requirements.txt` — Python dependencies.
- `Streamlit Interface.png` and `Streamlit Interface (2).png` — application screenshots.
