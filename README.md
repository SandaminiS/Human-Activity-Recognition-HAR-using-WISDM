# Human Activity Recognition (HAR) using WISDM: Deep Learning Approaches

## Overview
This project, completed for **CAP 5610: Machine Learning**, focuses on **Human Activity Recognition (HAR)** using the **WISDM** wearable/smartphone sensor dataset. We classify **18 daily activities** from accelerometer/gyroscope signals collected from smartphones and smartwatches, and compare multiple deep learning architectures.

---

## Group Members (Group 15)
- **Thiwanka Dissanayaka (Coordinator)** 
- **Shahd Alnofaie**  
- **Chathura Keshan** 
- **Sandamini Senaratne**  
- **Zack Willis**   

---

## Objectives
- Build a multi-class classifier to recognize **18 human activities** from wearable sensor signals.
- Evaluate and compare deep learning models for sequential/sensor data:
  - **MLP, CNN, RNN, BiLSTM, TCN**
- Analyze misclassifications and identify challenges (e.g., overlapping activities such as *eating soup* vs *eating pasta*).

---

## Dataset
- **Dataset:** WISDM (Fordham University)
- **Participants:** 51
- **Activities:** 18
- **Duration per activity:** 3 minutes
- **Sampling rate:** 20 Hz (every 50 ms)
- **Sensors:** Smartphone + Smartwatch (accelerometer + gyroscope)
- **Scale:** 15,630,426 raw measurements (with activity labels)

### Activity Classes (18)
Walking, Jogging, Stairs, Sitting, Standing, Typing, Brushing Teeth, Eating Soup, Eating Chips, Eating Pasta, Drinking from Cup, Eating Sandwich, Kicking (Soccer Ball), Playing Catch (Tennis Ball), Dribbling (Basketball), Writing, Clapping, Folding Clothes.

---

## Data Description / Representation
- Each activity is recorded at ~20 Hz for 3 minutes → **3,600 samples per axis (x, y, z)** per sensor.
- For implementation, data was structured into sequences with **19,800 features per sample**.

---

## Methodology

### Models Implemented
- **Multilayer Perceptron (MLP)**
- **Convolutional Neural Network (CNN)**
- **Recurrent Neural Network (RNN)**
- **Bidirectional LSTM (BiLSTM)**
- **Temporal Convolutional Network (TCN)**

### Hyperparameter Tuning
Hyperparameters were tuned using a systematic search (grid search with cross-validation), exploring:
- learning rate, dropout, kernel size, dilation factors, number of filters/hidden units, etc.

---

## Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-score  


