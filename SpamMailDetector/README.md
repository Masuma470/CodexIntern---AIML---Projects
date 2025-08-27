Spam Mail Detector
Project Overview

The Spam Mail Detector is a machine learning project that classifies emails as Spam or Not Spam using the Spambase dataset from UCI. The project demonstrates an end-to-end workflow from data exploration, preprocessing, model training, evaluation, and saving the trained model for future predictions.

Features

Binary classification of emails: Spam (1) / Not Spam (0)

Data preprocessing including feature scaling

Logistic Regression model for classification

Performance evaluation using Accuracy, Confusion Matrix, and Classification Report

Plots for confusion matrix and class distribution

Saving and loading of trained model and scaler for real-world usage

Project Highlights

End-to-End Workflow: Complete pipeline from data loading, exploration, preprocessing, to model training, evaluation, and deployment.

Practical & Deployable: Trained model and scaler are saved and can be reused for real-time spam detection without retraining.

Visualization-Driven Insights: Includes confusion matrix and class distribution plots to better understand data balance and model performance.

Reproducible & Well-Organized: Clear folder structure with data/, plots/, and models/ ensures the project is easy to navigate and reproduce.

High-Quality Evaluation: Model performance assessed using accuracy, precision, recall, F1-score, and confusion matrix, ensuring reliable spam detection.

Professional Documentation: Well-commented Jupyter Notebook with Markdown explanations for every step, making it easy for others to understand and present.

Folder Structure
spam_mail_detector/
├─ data/
│  ├─ spambase.data         # Dataset
│  └─ spambase.names        # Feature reference
├─ plots/
│  ├─ confusion_matrix.png
│  └─ class_distribution.png
├─ models/
│  ├─ spam_classifier.pkl   # Trained model
│  ├─ scaler.pkl             # StandardScaler
│  └─ metadata.json          # Model info & metrics
├─ notebook.ipynb           # Jupyter Notebook with steps 1-9
└─ README.md                # Project description

Getting Started
Prerequisites

Python 3.x

Jupyter Notebook

Required Libraries:

pandas
numpy
matplotlib
seaborn
scikit-learn
joblib
json

How to Run

Open notebook.ipynb in Jupyter Notebook.

Ensure the data/, plots/, and models/ folders exist.

Run all cells sequentially from Step 1 to Step 9.

Check the plots/ folder for saved visualizations.

Use the saved model and scaler in models/ to predict new emails.

Key Takeaways

Logistic Regression is effective for binary classification tasks like spam detection.

Preprocessing (like scaling features) improves model performance.

Saving the model and scaler enables real-world deployability.

Visualizations provide clear insights into model performance and data distribution.