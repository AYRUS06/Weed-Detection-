# Weed-Detection-
This project explores various state-of-the-art object detection techniques for identifying weeds in crop fields. Using high-resolution images from the Chicory Plant and Lincoln Beet datasets, YOLO versions emerged as the most effective model, delivering the best results for precise weed detection and improved agricultural efficiency.

# Weed Detection in Crop Fields

## Introduction
The presence of weeds in agricultural fields is one of the major challenges in crop productivity. This project leverages convolutional neural networks (CNNs) to automate the process of weed detection in crops. It outlines the methods followed, results obtained, and discusses implementation.

## Purpose
The primary purpose of employing machine learning techniques in agriculture is to automate the labor-intensive and time-consuming task of weed detection in agricultural fields. This can help:
- Reduce costs by enabling targeted weed control and minimizing unnecessary herbicide use.
- Lower labor costs.

## System Overview
The weed detection system processes high-resolution images of fields using CNN models to extract features. These features are passed to a pre-trained CNN model for weed detection. The output consists of bounding boxes that pinpoint the location of weeds in the field.

## Problem Statement
Weeds are undesirable plants that negatively impact crop growth and productivity. Differentiating between weeds and crops can be challenging, often leading to incorrect herbicide application, crop damage, or environmental harm. Conventional methods of weed control are labor-intensive, time-consuming, and environmentally harmful.

## Goal and Vision
The goal of this project is to accurately identify and distinguish between weeds and crops. This allows for precise actions to be taken, conserving resources and protecting the environment.

---

## Current Progress

### Dataset
- **Chicory Plant Dataset**
- **Lincoln Beet Dataset**

### Approaches
1. **Custom CNN Models**
   - Model with 7 CNN layers trained for 10 epochs achieved ~80% accuracy.
   - Model with 12 CNN layers trained for 10 epochs achieved ~88% accuracy.

2. **Transfer Learning**
   - Using EfficientNet-B0, transfer learning achieved an accuracy of more than 96%.

3. **Object Detection**
   - Implemented based on the paper: "Deep Object Detection of Crop Weeds: Performance of YOLOv7 on a Real Case Dataset from UAV Images".

### Results
#### Chicory Plant Dataset
| Model     | Backbone            | Precision | Recall | mAP50 | mAP50-95 |
|-----------|---------------------|-----------|--------|-------|----------|
| YOLOv8m   | CSPDarknet-53 (Elan) | 0.718     | 0.676  | 0.747 | 0.292    |
| YOLOv8n   | CSPDarknet-53 (Elan) | 0.651     | 0.526  | 0.583 | 0.178    |
| YOLOv7m   | Elan                | 0.640     | 0.513  | 0.555 | 0.145    |

#### Lincoln Beet Dataset
| Model     | Backbone            | Precision | Recall | mAP50 | mAP50-95 |
|-----------|---------------------|-----------|--------|-------|----------|
| YOLOv8m   | CSPDarknet-53       | 0.652     | 0.864  | 0.746 | 0.618    |
| YOLOv8n   | CSPDarknet-53       | 0.544     | 0.670  | 0.678 | 0.345    |

### Observations
- Results on the Chicory Plant Dataset are promising.
- Model performance on the Lincoln Beet Dataset requires improvement.

---

Feel free to explore the code, datasets, and results in this repository. Contributions and suggestions are welcome!
