Analysis of Chest X-Ray Images Using Machine Learning
Project Overview
This project is focused on developing a machine learning model to classify chest X-ray images into two categories: 'Normal' and 'Pneumonia'. The model aims to assist in the rapid diagnosis of pneumonia by analyzing chest X-ray images, which can lead to timely treatment and improved patient outcomes.

Course Information
Course Name: Data Mining and Foundation of AI (6CC555)
Student Number: 100610788
Objective
The main objective of this project is to develop a Convolutional Neural Network (CNN) model capable of accurately differentiating between normal and pneumonia conditions in chest X-rays. This can significantly improve the speed and accuracy of pneumonia diagnosis.

Dataset
Source: The dataset was obtained from Kaggle and contains labeled chest X-ray images categorized as 'Normal' and 'Pneumonia'.
Dataset Link: Kaggle Chest X-Ray Pneumonia Dataset
Volume: Thousands of X-ray images provide a robust basis for training the diagnostic model.

Data Preparation
Data Cleaning: Checked for any corrupted images or unusual file sizes that might affect model training.
Preprocessing:
Resizing: All images were resized to a uniform size to ensure consistent input data.
Normalization: Pixel values were scaled to the [0,1] range for faster convergence during training.
Model Architecture
Type: Convolutional Neural Network (CNN)
Components:
Convolutional layers, activation functions (ReLU), pooling layers, and dense layers.
Number of Parameters: 2,507,618 trainable parameters.
Data Split: The dataset was divided into training and testing sets to accurately evaluate model performance.

Training Process
Hardware: Model training was performed using both CPU and GPU, with no notable differences in the results.
Epochs: The model was trained for 30 epochs using batches of images.
Data Augmentation: Techniques such as rotations and shifts were applied to improve model robustness.
Model Saving: The model and its training history were saved for future use and easy retraining.
Exploratory Data Analysis (EDA)
Visualization: Sample X-ray images were visually inspected to understand the key characteristics and variations in the dataset.
Class Distribution: Ensured that the dataset had a balanced representation of both 'Normal' and 'Pneumonia' images to minimize bias.

Model Evaluation
Performance Metrics:
Confusion Matrix: High true positives and true negatives indicate strong predictive ability.
Loss and Accuracy Graphs: Training loss decreases sharply, but validation loss suggests potential overfitting after the initial epochs.
Model Insights:
Grad-CAM Visualizations: Highlighted lung fields in X-rays, showing the model effectively focused on areas crucial for pneumonia diagnosis.

Advanced Techniques
LIME (Local Interpretable Model-Agnostic Explanations): Applied to make the model's decision-making process transparent by identifying which parts of the image influenced predictions.
Grad-CAM: Provided heatmap visualizations of the lung regions, validating that the model focuses on relevant anatomical areas for pneumonia diagnosis.
