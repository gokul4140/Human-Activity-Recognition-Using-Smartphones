# Human-Activity-Recognition-Using-Smartphones
This project focuses on recognizing human activities using smartphone sensor data. The implementation combines machine learning techniques to classify activities effectively.

## Overview
Human Activity Recognition (HAR) is an essential field in modern technology with applications ranging from healthcare to fitness tracking. This project uses a machine learning pipeline that leverages **KMeans clustering** for dimensionality reduction and **Naive Bayes** classification for activity recognition.

## Dataset
The dataset contains recordings of 30 participants performing daily activities while carrying a waist-mounted smartphone equipped with accelerometer and gyroscope sensors. Each data sample includes time- and frequency-domain features extracted from the raw sensor signals.

## Implementation Details
### 1. Dimensionality Reduction using KMeans
- **Why KMeans?**  
  To reduce the feature space by clustering similar features and selecting representative ones, improving computation efficiency while retaining meaningful patterns in the data.
- **Steps:**
  - Transpose the dataset to treat features as data points.
  - Apply KMeans clustering to group similar features into clusters.
  - Select one representative feature from each cluster for further classification.
### 2. Classification using Naive Bayes
- **Why Naive Bayes?**  
  Its simplicity and effectiveness for multiclass classification tasks make it suitable for this problem. Despite its assumption of feature independence, it often performs well on sensor-based data.
- **Steps:**
  - Train the Naive Bayes classifier on the reduced feature set obtained from KMeans.
  - Predict activity labels for new data samples.
## Results
The model achieves competitive accuracy with a lightweight design, making it suitable for real-time applications on resource-constrained devices.
