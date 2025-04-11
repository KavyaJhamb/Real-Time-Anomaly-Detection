# Real-Time Anomaly Detection in IoT-Enabled Smart Grids: A Comparative Study of Autoencoders and GANs

Overview
This repository contains the implementation of Autoencoder and Generative Adversarial Network (GAN) models for real-time anomaly detection in IoT-enabled smart grids. The project focuses on identifying anomalies such as cyberattacks, equipment malfunctions, and operational inefficiencies by analyzing reconstruction errors. The research compares the performance of both models in terms of accuracy, scalability, and computational efficiency, providing valuable insights into their practical applications for smart grid security and reliability.
Features
Autoencoder Model:
Detects anomalies based on reconstruction error.
Suitable for detecting operational anomalies like equipment overloads and faults.
Computationally efficient with stable training behavior.
GAN Model:
Learns the full distribution of normal data using adversarial training.
Detects anomalies caused by environmental and market factors (e.g., humidity, electricity pricing).
Provides higher precision but requires more computational resources.
Hybrid Framework Proposal:
Combines the strengths of Autoencoders (high recall) and GANs (high precision).
Suggests ensemble detection and cascaded thresholding for optimal performance.
Key Contributions
Comparative analysis of Autoencoder and GAN models for anomaly detection in smart grids.
Feature-level error attribution analysis to identify root causes of anomalies.
Evaluation of model performance using metrics such as Precision, Recall, F1 Score, and ROC-AUC.
Insights into hybrid frameworks that leverage the strengths of both approaches.
Dataset Details
The dataset used in this study was collected from IoT sensors deployed in a simulated smart grid environment. It includes over 50,000 timestamped entries across 10 operational and environmental parameters (e.g., voltage, current, humidity). Due to confidentiality agreements, the dataset is not publicly available; however, synthetic anomalies were injected into the test set to evaluate model performance.
Installation
To replicate this project locally, follow these steps:
Clone the repository:
bash
git clone https://github.com/your-username/real-time-anomaly-detection.git
cd real-time-anomaly-detection
Install dependencies:
bash
pip install -r requirements.txt
Run the models:
Train the Autoencoder:
bash
python train_autoencoder.py
Train the GAN:
bash
python train_gan.py
Evaluate performance:
bash
python evaluate_models.py
Results
Performance Metrics Comparison
Metric	Autoencoder	GAN
Precision	0.1153	0.1368
Recall	0.0126	0.0545
F1 Score	0.0227	0.0779
The Autoencoder demonstrated higher recall, making it suitable for broad anomaly detection.
The GAN achieved higher precision, reducing false positives but missing subtle anomalies.
Visualizations:
Reconstruction Error Distribution (Autoencoder & GAN).
ROC Curves comparing model sensitivity and specificity.
Future Research Directions
Develop hybrid frameworks combining Autoencoders and GANs for improved anomaly detection across diverse scenarios.
Optimize models for edge computing environments using techniques like quantization and pruning.
Explore robustness against adversarial attacks targeting IoT-enabled smart grids.
Validate models on geographically diverse datasets to ensure generalizability.
