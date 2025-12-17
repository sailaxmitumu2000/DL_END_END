# DL_END_END
📌 Project Overview
This project implements an end-to-end deep learning pipeline for Kidney Disease Classification using Convolutional Neural Networks (CNNs), following production-grade MLOps practices.
Unlike notebook-based experiments, this repository is structured to reflect how real-world machine learning systems are built, tracked, versioned, and deployed.
The project covers the complete ML lifecycle — from data ingestion to model training, evaluation, experiment tracking, reproducibility, and deployment readiness.
🎯 Problem Statement
Early and accurate detection of kidney disease is critical for effective treatment.
This project aims to classify medical images into kidney disease categories using a CNN-based deep learning approach, while ensuring the solution is scalable, reproducible, and production-ready.
🧠 Solution Approach
Used transfer learning with a pretrained CNN backbone to leverage learned visual features
Designed a modular pipeline architecture, separating each ML stage into independent components
Enabled configuration-driven experimentation using YAML files
Integrated MLOps tools to ensure reproducibility and experiment traceability
⚙️ Project Workflow
The pipeline is divided into the following stages:
Data Ingestion
Automated download and extraction of the dataset
Stored outputs as versioned artifacts
Prepare Base Model
Loaded pretrained CNN architecture
Froze base layers to reduce training complexity
Added a custom classification head
Model Training
Trained only the custom layers for efficiency
Logged metrics and parameters during training
Model Evaluation
Evaluated performance on validation/test data
Saved evaluation metrics for comparison
Experiment Tracking (MLflow)
Logged hyperparameters, metrics, and trained models
Enabled comparison across multiple experiment runs
Data & Artifact Versioning (DVC)
Version-controlled datasets and pipeline outputs
Ensured full reproducibility across experiments
Prediction Pipeline
Built an inference pipeline for model predictions
Prepared a user-facing prediction workflow
Deployment Readiness
Containerized the application using Docker
Designed the workflow for AWS-based CI/CD deployment
🛠️ Tools & Technologies
Programming Language: Python
Deep Learning: TensorFlow / Keras
Model Architecture: CNN with Transfer Learning
Experiment Tracking: MLflow
Data & Artifact Versioning: DVC
Configuration Management: YAML
Containerization: Docker
Cloud Deployment: AWS (CI/CD ready)
📈 Key Learnings
Machine learning systems require engineering discipline, not just model accuracy
MLflow enables structured and comparable experimentation
DVC ensures data and artifact reproducibility across runs
Modular pipelines significantly improve scalability and maintainability
End-to-end MLOps practices are essential for production ML systems
