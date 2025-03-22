# Driver Drowsiness Detection

## Overview
This project focuses on detecting driver drowsiness using deep learning techniques, specifically **CNN (Convolutional Neural Networks) and LSTM (Long Short-Term Memory)** networks. The model is trained on the **Driver Drowsiness Dataset (DDD)**, which consists of extracted facial images of drivers categorized into **Drowsy** and **Non-Drowsy** states.

## Dataset
**Driver Drowsiness Dataset (DDD)** is derived from the Real-Life Drowsiness Dataset. The dataset contains **cropped face images** of drivers extracted from videos using **VLC software** and further processed using the **Viola-Jones algorithm** to detect the **Region of Interest (ROI)**.

### Dataset Properties:
- **Image Type**: RGB
- **Classes**: 2 (Drowsy & Non-Drowsy)
- **Image Size**: 227 x 227 pixels
- **Total Images**: Over 41,790 images
- **Dataset Link**: [Kaggle - Driver Drowsiness Dataset](https://www.kaggle.com/datasets/ismailnasri20/driver-drowsiness-dataset-ddd)

## Methodology
The model utilizes a combination of **CNN and LSTM** for effective feature extraction and temporal sequence learning:
1. **CNN (Convolutional Neural Networks)**:
   - Extracts spatial features from images.
   - Helps in recognizing patterns related to drowsiness.
2. **LSTM (Long Short-Term Memory)**:
   - Captures temporal dependencies between frames.
   - Enhances accuracy by learning sequential patterns of drowsiness.

## Model Training
- **Preprocessing**:
  - Resized images to **227x227 pixels**.
  - Normalized pixel values.
- **Architecture**:
  - **CNN layers** for feature extraction.
  - **LSTM layers** for sequence modeling.
  - **Fully connected layers** with a softmax activation for classification.
- **Training Details**:
  - Optimizer: **Adam**
  - Loss Function: **Categorical Cross-Entropy**
  - Batch Size: **32**
  - Number of Epochs: **25-50 (Tuned for optimal performance)**

## Results
- Achieved high accuracy in classifying drowsy vs. non-drowsy states.
- Improved detection speed and reliability compared to traditional methods.

