
# SAMARITANS

## Overview

**SAMARITANS** is a machine learning project aimed at predicting hospital readmissions for heart failure patients. Utilizing the MIMIC-III dataset, the project implements various classification models to identify patients at risk of readmission, thereby assisting healthcare providers in proactive patient care.

## Project Structure

- **`Readmission_Heart_Patients_Modelling.ipynb`**: Jupyter notebook containing data preprocessing, model training, evaluation, and prediction steps.
- **`DATASETS/RAW_DATA_MIMIC_III.zip`**: Compressed file containing the raw dataset extracted from the MIMIC-III database.
- **`DATASETS/Data_predictions.csv`**: CSV file with model predictions on the test dataset.

## Implementation in Google Colab

The project is designed to run seamlessly on [Google Colab](https://colab.research.google.com/github/abd766/SAMARITANS/blob/main/Readmission_Heart_Patients_Modelling.ipynb), providing an accessible environment for executing the notebook without local setup complexities.

### Steps to Run:

1. Upload the notebook `Readmission_Heart_Patients_Modelling.ipynb` to Google Drive.
2. Open it with Google Colab.
3. Mount Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
4. Navigate to dataset directory:
   ```python
   %cd /content/drive/MyDrive/path_to_dataset_directory
   ```
5. Execute the notebook cells sequentially to preprocess, train, and predict.

## Models Used

This project experiments with the following models:

- **Logistic Regression**
- **Random Forest Classifier**
- **Support Vector Machine (SVM)**
- **Gradient Boosting Classifier**
- **XGBoost Classifier**

Model performance is evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score

## Dataset

The dataset is derived from the **MIMIC-III (Medical Information Mart for Intensive Care III)** database and includes:

- Patient demographics (age, gender, ethnicity)
- Hospitalization data (admission type, length of stay)
- Medical history
- Readmission labels (binary)

Preprocessing steps include handling missing values, encoding categorical variables, and standardization.

## Predictions

Predictions made by trained models include:

- **Binary Readmission Labels** (`0` or `1`)
- **Probability Scores**

These are stored in:
- `DATASETS/Data_predictions.csv`

They can be used for risk stratification and early interventions.

## Getting Started

```bash
git clone https://github.com/abd766/SAMARITANS.git
```

- Extract the training and testing dataset from  `DATASETS`
- Open the notebook in Google Colab
- Follow the cell-by-cell instructions

## Acknowledgments

- **MIMIC-III** for the dataset
- **Google Colab** for notebook execution
