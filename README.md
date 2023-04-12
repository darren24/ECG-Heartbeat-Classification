# ECG Heartbeat Classification (https://ecgbeat.herokuapp.com)
This project aims to classify ECG beats into different types using machine learning techniques. ECG (Electrocardiogram) is a diagnostic tool that measures and records the electrical activity of the heart in exquisite detail. By analyzing ECG signals, medical professionals can detect various heart-related abnormalities.

## Problem Statement
The goal is to develop a machine learning model that can accurately classify ECG beats into one of the five following classes:

Normal beat (N)
Atrial premature beat (APB)
Left bundle branch block beat (LBBB)
Right bundle branch block beat (RBBB)
Premature ventricular contraction (PVC)
Dataset
The dataset used for this project is the MIT-BIH Arrhythmia Dataset, which contains 48 half-hour excerpts of two-channel ambulatory ECG recordings from 47 subjects, annotated beat-by-beat.
## Please refer to the ECG_Classification.ipynb file for all the work done on this project.

## Data Preprocessing
Before training the model, the dataset was preprocessed to ensure the best possible results. The preprocessing steps included:

1. Signal filtering: Remove high-frequency noise and baseline wander using Butterworth filters.
2. R-peak detection: Identify the R-peaks in the ECG signal to segment individual heartbeats.
3. Feature extraction: Extract relevant features from the ECG beats that can be used as input for the machine learning model.

## Model Training
Various machine learning algorithms were evaluated, including:

1. Random Forest
2. Support Vector Machines
3. Convolutional Neural Network
4. Long Short-Term Memory (LSTM)
After comparing their performance, the best model was selected based on metrics such as accuracy, precision, recall, and F1 score.

## Model Evaluation
The chosen model was evaluated using cross-validation and a hold-out test set. The performance metrics (accuracy, precision, recall, F1 score) were calculated to determine the effectiveness of the model in classifying ECG beats.

## Web App
A web application was developed to provide an easy-to-use interface for users to interact with the ECG heartbeat classification model. Users can upload their ECG data files and get real-time predictions of the ECG beat types.
To check out the Web app go to the link https://ecgbeat.herokuapp.com

## Dependencies
Python 3.7+
pandas
numpy
scipy
scikit-learn
matplotlib
Flask
Usage

## Conclusion
This project demonstrates the potential of using machine learning for automated ECG beat classification, which can aid medical professionals in diagnosing and monitoring various heart-related conditions.
