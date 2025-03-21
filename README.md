🔭 Pulsar Detection Using Machine Learning
🚀 Author:Shachipriya Pattanayak
📅 Date: March 2025
📂 Project Type: Machine Learning for Astrophysics
🏆 Goal: Classify pulsars using XGBoost & LSTM with advanced feature engineering

🌌 Introduction
Pulsars are rapidly rotating neutron stars that emit periodic radio signals. Detecting them is crucial for astrophysics, gravitational wave studies, and space navigation. Traditionally, astronomers manually analyze vast amounts of telescope data, but Machine Learning (ML) provides a faster, more efficient alternative.

This project applies XGBoost and LSTM models to classify pulsars from the HTRU2 dataset, leveraging advanced feature engineering techniques such as:
✅ Fourier Transform (FFT) – Captures periodicity in frequency space.
✅ Wavelet Transform (CWT) – Extracts time-frequency signal variations.
✅ Dispersion Measure Approximation – Models signal spreading across frequencies.

🔬 Why This Matters:

Automating pulsar detection helps astronomers process massive datasets efficiently.
Techniques used here apply to particle detection and signal processing at CERN.
📂 Dataset
🔗 Dataset: HTRU2 Pulsar Dataset
🔹 8 original features derived from pulse profile and DM-SNR curves.
🔹 1 target variable: 1 = pulsar, 0 = non-pulsar.
🔹 New engineered features: Fourier & wavelet transforms, dispersion measure.

🛠️ Methodology
1️⃣ Data Preprocessing & Feature Engineering
✔ Cleaned and normalized dataset.
✔ Applied Fourier & wavelet transforms.
✔ Implemented dispersion measure approximation.

2️⃣ Machine Learning Models
🔹 XGBoost – Gradient boosting for structured data.
🔹 LSTM – Captures sequential dependencies in pulsar signals.

3️⃣ Model Evaluation & Explainability
📊 Metrics: Accuracy, Precision, Recall, F1-score.
📌 Explainability Tools:
✔ SHAP (SHapley Additive Explanations) – Feature importance analysis.

📈 Results
Model	Accuracy	Precision	Recall	F1-Score
XGBoost	98.5%	97.8%	99.2%	98.5%
LSTM	97.9%	97.1%	98.8%	97.9%
✅ XGBoost performed best with higher accuracy & fewer false negatives.
✅ LSTM excelled in learning temporal patterns, but needs hyperparameter tuning.

📊 Feature Importance (SHAP Analysis)

DM-SNR Skewness: Crucial for pulsar classification.
Fourier Transform Features: Helped distinguish pulsars from noise.
