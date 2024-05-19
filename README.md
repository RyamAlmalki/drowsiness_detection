![Drowsiness Detection](https://media.giphy.com/media/BD4DIGsIhkOZ2lI0v1/giphy.gif)


# Drowsiness Detection 👁️👀

Welcome to the Drowsiness Detection System! This project aims to determine whether eyes are open or closed using image processing and machine learning techniques. It integrates facial landmark detection with the Eye Aspect Ratio (EAR) to create a comprehensive dataset. Using this data, we train machine learning models to achieve high accuracy in eye state detection.

## Table of Contents 📋
- [Overview](#overview-)
- [Features](#features-)
- [Usage](#usage-)
- [Dataset Preparation](#dataset-preparation-)
- [Model Training](#model-training-)
- [Contributing](#contributing-)

## Overview 🌟
This project combines facial landmark detection with EAR calculation to create a dataset of images categorized as having 'opened eyes' or 'closed eyes'. Two models are implemented:
- **SVM (Support Vector Machine)**: A traditional machine learning model.
- **CNN (Convolutional Neural Network)**: A deep learning model for higher accuracy.

## Features ✨
- **Facial Landmark Detection**: Uses dlib's pre-trained facial landmark detector.
- **Eye Aspect Ratio (EAR)**: Calculates EAR to determine eye openness.
- **Data Preprocessing**: Includes adaptive histogram equalization, Gaussian blur, and edge enhancement.
- **Model Training**: Implements both SVM and CNN models.

## Usage 🚀
1. **Build the dataset**:
    - Ensure you have images of both open and closed eyes in the respective directories.
    - Run the dataset building script to label and preprocess the images.

2. **Train the models**:
    - Use the provided scripts to train the SVM and CNN models on the prepared dataset.

3. **Evaluate the models**:
    - Evaluate the trained models using cross-validation and ROC curve analysis.

## Dataset Preparation 📊
1. **Image Preprocessing**: Convert images to grayscale, apply adaptive histogram equalization, Gaussian blur, and edge enhancement.
2. **EAR Calculation**: Use facial landmarks to calculate EAR and label images as 'open' or 'closed'.
3. **Data Augmentation**: Optionally, augment the dataset to improve model robustness.

## Model Training 📈
- **SVM**: Uses a linear kernel SVM with EAR as an additional feature.
- **CNN**: A deep learning model combining image data and EAR for improved accuracy.

## Contributing 🤝
We welcome contributions to enhance this project! To contribute, please:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.
