# Human Activity Recognition Using Vision-Based Features

## Introduction
This project explores a vision-based approach for Human Activity Recognition (HAR) without requiring sensors or wearables. It focuses on recognizing three activities—Eating, Walking, and Chitchat—using computer vision and machine learning techniques. The model has applications in surveillance, elder care, healthcare monitoring, and human-robot interaction.

## Project Overview
The system is designed to:

1. **Collect and preprocess image data.**
2. **Extract robust features** using BRISK, SIFT, and their fusion.
3. **Apply machine learning classifiers** to achieve high accuracy.

The fusion of BRISK and SIFT descriptors, a novel approach, demonstrated superior performance compared to standalone descriptors.

### Key Features
- **Input:** Image dataset of 1,306 images divided across three classes.
- **Output:** Activity classification with high accuracy.
- **Tools Used:** Python, OpenCV, Scikit-learn.

## Workflow

### 1. Data Collection
Gather images of activities in various formats.

### 2. Preprocessing
- Resize images to a uniform size.
- Convert images to grayscale.
- Remove background using deep learning-based methods.
- Apply edge detection using Prewitt filters.

### 3. Feature Extraction
- Extract features using BRISK, SIFT, and ORB descriptors.
- Perform feature fusion (BRISK + SIFT) for enhanced performance.

### 4. Clustering and Classification
- Use K-means for dimensionality reduction.
- Train classifiers (e.g., Random Forest) for activity recognition.

## Results
The model achieved an accuracy of **89.41%** using the Random Forest classifier with the fused BRISK and SIFT descriptors.

### Performance Comparison
| Descriptor | Classifier     | Accuracy |
|------------|----------------|----------|
| BRISK      | Random Forest  | 86.98%   |
| SIFT       | Random Forest  | 85.32%   |
| ORB        | Random Forest  | 83.74%   |
| Fusion     | Random Forest  | **89.41%** |

## Conclusion
This project successfully demonstrates a vision-based approach for Human Activity Recognition using a novel fusion of BRISK and SIFT features. The system achieves a high accuracy of 89.41% with the Random Forest classifier, showcasing its effectiveness and potential applications in surveillance, elder care, and activity monitoring. With future enhancements, such as a larger dataset and real-time deployment, the model can be extended to broader use cases and achieve even greater performance.

## Published Work
For more details, refer to the published paper: [Human Activity Recognition Using Vision-Based Features](https://ieeexplore.ieee.org/document/10199987).
