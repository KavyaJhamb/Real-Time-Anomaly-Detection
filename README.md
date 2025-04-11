# Real-Time Anomaly Detection in IoT-Enabled Smart Grids: A Comparative Study of Autoencoders and GANs

A Comparative Study of Autoencoders and GANs

📌 Overview

This repository contains the implementation of Autoencoder and Generative Adversarial Network (GAN) models for real-time anomaly detection in IoT-enabled smart grids. The primary goal is to identify anomalies such as cyberattacks, equipment malfunctions, and operational inefficiencies by analyzing reconstruction errors.
This study provides a comparative analysis of both models based on accuracy, scalability, and computational efficiency, offering insights into their practical applications for enhancing smart grid security and reliability.

🚀 Features

🔹 Autoencoder Model
Detects anomalies based on reconstruction error.
Best suited for identifying operational anomalies like equipment faults or overloads.
Lightweight and computationally efficient with stable training dynamics.

🔹 GAN Model
Learns the distribution of normal behavior through adversarial training.
Excels in detecting contextual anomalies (e.g., due to environmental or market shifts).
Offers higher precision but is computationally more intensive.

🔹 Hybrid Framework (Proposed)
Leverages the high recall of Autoencoders and the high precision of GANs.
Implements ensemble detection and cascaded thresholding to optimize performance.

🧠 Key Contributions

In-depth comparison of Autoencoder and GAN models for anomaly detection in smart grids.
Feature-level error attribution analysis to trace the root cause of anomalies.
Evaluation using key metrics: Precision, Recall, F1 Score, and ROC-AUC.
Proposal of a hybrid detection framework combining both model strengths.

📊 Dataset Details

The dataset originates from IoT sensors in a simulated smart grid environment.
Includes 50,000+ timestamped entries across 10 features like voltage, current, and humidity.
Due to confidentiality agreements, the original dataset is not publicly available.
Synthetic anomalies were injected into the test set for robust performance evaluation.

⚙️ Installation & Usage
1. Clone the Repository
git clone https://github.com/your-username/real-time-anomaly-detection.git
cd real-time-anomaly-detection
2. Install Dependencies
pip install -r requirements.txt
3. Train the Models
▫️ Train the Autoencoder
python train_autoencoder.py
▫️ Train the GAN
python train_gan.py
