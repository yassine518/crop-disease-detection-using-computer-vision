# Crop Disease Detection

## Overview
This project tackles crop disease detection using computer vision and object detection techniques. The goal is to identify and localize various plant diseases in agricultural images to help farmers detect crop health issues early.

## Approach
- **Model**: Implemented YOLOv8 medium model for object detection
- **Dataset**: Ghana crop disease dataset with multiple disease classes (excluding corn-related diseases)
- **Cross-validation**: Used 20-fold stratified cross-validation for robust model evaluation
- **Image preprocessing**: Images resized to 1024x1024 resolution
- **Data augmentation**: Applied various augmentation techniques including horizontal/vertical flips, rotation, translation, scaling, and HSV adjustments
- **Training configuration**: 40 epochs with early stopping, batch size of 12, and cosine learning rate scheduling

## Key Features
- Multi-class disease detection across different crop types
- Comprehensive data augmentation pipeline
- Stratified k-fold validation to ensure balanced training/validation splits
- Custom evaluation metrics using mean Average Precision (mAP)

## Results
Achieved a **mean average precision (mAP) of 0.47**, ranking **36th out of 345 participants** in the competition.

## Technical Stack
- **Framework**: Ultralytics YOLOv8
- **Libraries**: PyTorch, OpenCV, scikit-learn, pandas
- **Tracking**: Weights & Biases for experiment monitoring