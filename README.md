# Deep Learning-Based Predictive Maintenance for Induction Motors Using Hybrid CNN-LSTM Architecture with Attention Mechanism

## Overview

This project presents an intelligent Predictive Maintenance System for induction motors using a Hybrid CNN-LSTM Deep Learning Architecture enhanced with an Attention Mechanism. The system is designed to detect and classify motor faults from vibration signal data, enabling proactive maintenance and reducing unplanned downtime in industrial environments.

The proposed framework combines the feature extraction capabilities of Convolutional Neural Networks (CNNs) with the temporal sequence learning power of Long Short-Term Memory (LSTM) networks. An attention layer further improves performance by focusing on the most informative temporal patterns in sensor data.

Additionally, an interactive Plotly Dash dashboard has been developed for real-time monitoring, fault visualization, prediction analysis, and maintenance recommendations.

---

## Key Features

* Hybrid CNN-LSTM architecture with Attention Mechanism
* Multi-scale CNN feature extraction using parallel convolution branches
* Bidirectional LSTM for temporal pattern learning
* Automated fault classification of induction motors
* Time-domain, frequency-domain, and wavelet-based feature engineering
* Real-time monitoring dashboard using Plotly Dash
* Interactive fault analytics and maintenance recommendations
* High-performance multi-class fault diagnosis system
* Industrial predictive maintenance workflow simulation

---

## Problem Statement

Industrial induction motors are prone to various faults such as:

* Bearing Faults
* Broken Rotor Bar Faults
* Stator Faults
* Voltage Unbalance
* Overload Conditions

Traditional maintenance approaches often lead to unnecessary servicing or unexpected failures. This project aims to provide a data-driven predictive maintenance solution capable of identifying faults before catastrophic failures occur.

---

## Dataset

The model is trained using the Fault Induction Motor Dataset containing six operational conditions:

| Class | Description        |
| ----- | ------------------ |
| 0     | Normal Operation   |
| 1     | Bearing Fault      |
| 2     | Broken Rotor Bar   |
| 3     | Stator Fault       |
| 4     | Voltage Unbalance  |
| 5     | Overload Condition |

---

## System Architecture

### Data Pipeline

1. Data Acquisition
2. Data Cleaning & Preprocessing
3. Feature Engineering
4. Model Training
5. Fault Prediction
6. Dashboard Visualization

### Hybrid CNN-LSTM Model

#### CNN Branch

Multi-scale feature extraction using:

* Kernel Size = 3
* Kernel Size = 5
* Kernel Size = 7

Each branch contains:

* Conv1D
* Batch Normalization
* Max Pooling
* Dropout

#### BiLSTM Branch

* Bidirectional LSTM Layers
* Attention Mechanism
* Temporal Dependency Learning

#### Feature Fusion

CNN and LSTM outputs are concatenated and passed through dense layers for fault classification.

---

## Feature Engineering

### Time-Domain Features

* Mean
* Standard Deviation
* RMS
* Peak Value
* Crest Factor
* Shape Factor
* Impulse Factor
* Signal Energy
* Skewness
* Kurtosis

### Frequency-Domain Features

* FFT-Based Features
* Dominant Frequency
* Spectral Centroid
* Spectral Spread
* Frequency Magnitudes

### Wavelet Features

* Multi-resolution signal analysis
* Fault signature extraction

---

## Model Performance

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 98.60% |
| Precision | 98.63% |
| Recall    | 98.60% |
| F1-Score  | 98.60% |
| ROC-AUC   | > 0.99 |

The model demonstrates excellent performance across all fault categories with near-perfect classification capability.

---

## Dashboard Features

The Predictive Maintenance Dashboard provides:

### System Monitoring

* Live Motor Status
* Fault Prediction Results
* Confidence Scores
* Remaining Useful Life Estimation

### Analytics

* Training Performance Visualization
* Class Distribution Analysis
* Confusion Matrix
* ROC Curves
* Feature Importance

### Fault Management

* Fault Database
* Historical Fault Records
* Trend Analysis

### Maintenance Management

* Maintenance Logs
* Cost Analysis
* Predictive Recommendations

---

## Technology Stack

### Programming Language

* Python 3.x

### Deep Learning

* TensorFlow
* Keras

### Data Processing

* NumPy
* Pandas
* SciPy
* Scikit-Learn

### Feature Engineering

* PyWavelets
* FFT Analysis

### Visualization

* Plotly
* Plotly Dash
* Dash Bootstrap Components

### Model Utilities

* Joblib

---

## Project Structure

```text
├── data/
│   ├── raw_data/
│   └── processed_data/
│
├── models/
│   ├── trained_model.keras
│   ├── feature_scaler.pkl
│
├── notebooks/
│   └── Deep Learning Based Predictive Maintenance.ipynb
│
├── dashboard/
│   └── dashboard.py
│
├── reports/
│   └── Project Report.pdf
│
├── results/
│   ├── confusion_matrix.png
│   ├── roc_curves.png
│   ├── training_history.png
│
├── requirements.txt
└── README.md
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/predictive-maintenance-cnn-lstm.git

cd predictive-maintenance-cnn-lstm
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Dashboard

```bash
python dashboard.py
```

Then open:

```text
http://127.0.0.1:8050/
```

in your browser.

---

## Future Enhancements

* Integration with real-time IoT sensors
* Edge AI deployment
* Digital Twin implementation
* Transfer Learning for fault adaptation
* Explainable AI (XAI) support
* Cloud-based monitoring platform
* Predictive Remaining Useful Life (RUL) estimation

---

## Research Contributions

* Novel Hybrid CNN-LSTM Architecture with Attention
* Multi-scale Feature Extraction Framework
* High-Accuracy Multi-Class Fault Classification
* Industrial Predictive Maintenance Dashboard
* End-to-End Deep Learning-Based Monitoring System

---

## Author

**Jackson Jacob L**

M.Tech Artificial Intelligence and Data Science

SRM Institute of Science and Technology

---

## License

This project is developed for academic and research purposes. Feel free to use and modify it for educational and non-commercial applications.

---

## Acknowledgements

Special thanks to the Department of Computational Intelligence, SRM Institute of Science and Technology, and all faculty members who provided guidance and support throughout this research work.
