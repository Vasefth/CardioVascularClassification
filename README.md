# CardioVascularClassification

# Heart Failure Prediction using Deep Learning

## Overview

This project focuses on predicting heart failure events using patient medical record data through a deep learning model. The dataset used (heart_failure.csv) comprises various medical attributes which are indicative of heart failure risks. This Python script utilizes libraries such as Pandas, Scikit-learn, and TensorFlow to preprocess the data, split it into training and testing sets, and finally, to build and evaluate a neural network model aimed at predicting heart failure events.

## Features

- Data preprocessing with Pandas and Scikit-learn.
- Data normalization and encoding.
- Training a deep learning model using TensorFlow.
- Evaluation of the model's performance.

## Dataset

The dataset heart_failure.csv must include the following columns:

- age: Age of the patient.
- anaemia: Decrease of red blood cells or hemoglobin (Boolean).
- creatinine_phosphokinase: Level of the CPK enzyme in the blood (mcg/L).
- diabetes: If the patient has diabetes (Boolean).
- ejection_fraction: Percentage of blood leaving the heart at each contraction.
- high_blood_pressure: If the patient has hypertension (Boolean).
- platelets: Platelets in the blood (kiloplatelets/mL).
- serum_creatinine: Level of serum creatinine in the blood (mg/dL).
- serum_sodium: Level of serum sodium in the blood (mEq/L).
- sex: Woman or man (Binary).
- smoking: If the patient smokes or not (Boolean).
- time: Follow-up period (days).
- death_event: If the event of death occurred (Boolean).

## Requirements

- Python 3.x
- Pandas
- Scikit-learn
- TensorFlow

## Setup

To run this project, install the above requirements using pip:

pip install pandas scikit-learn tensorflow

Ensure you have the heart_failure.csv dataset in your project directory.

## Usage

Execute the script with Python to train the model and evaluate its performance:

python heart_failure_prediction.py

The script will:

1. Load and preprocess the dataset.
2. Split the data into training and testing sets.
3. Normalize specific features and encode categorical variables.
4. Train a deep learning model on the training set.
5. Evaluate the model's accuracy on the testing set.
6. Print a classification report detailing the performance of the model.

## Model

The neural network model consists of:

- An input layer.
- Two hidden layers with 12 neurons each, using ReLU activation.
- An output layer with softmax activation to classify the prediction into two classes (death_event occurrences).

## Evaluation

After training, the script evaluates the model using the test set and prints a classification report, including precision, recall, f1-score, and accuracy metrics.

## Contributing

Feel free to fork this project, submit pull requests, or send suggestions to improve the code or the way the model handles the dataset.
