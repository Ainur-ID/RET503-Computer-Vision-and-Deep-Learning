# RET503 - Transfer Learning for Computer Vision

Project for RET503 Computer Vision and Deep Learning.

## Project Objective

This project applies transfer learning and fine-tuning for image classification using a pretrained ResNet18 model.

The experiment compares three training strategies:

1. Feature Extraction
2. Partial Fine-Tuning
3. Training from Scratch

## Project Pipeline

Camera
→ Camera Calibration
→ Undistortion
→ Image Preprocessing
→ Dataset
→ ResNet18
→ Classification
→ Latency Evaluation

## Dataset

The dataset will contain at least 50 images for each object class.

Each image will be collected under different:

- distances
- positions
- orientations
- lighting conditions
- backgrounds

## Training

Three ResNet18 configurations will be compared:

### Feature Extraction

- ImageNet pretrained weights
- Only final classification layer is trained
- Learning rate: 1e-3

### Partial Fine-Tuning

- ImageNet pretrained weights
- Layer4 and final classification layer are trained
- Learning rate: 1e-4 / 1e-3

### Training from Scratch

- Random initialization
- All layers are trained
- Learning rate: 1e-3

## Evaluation

The experiment will record:

- Validation accuracy
- Training time
- Epoch reaching 90% accuracy, if achieved
- Model latency

## Repository Structure

```text
RET503/
├── docs/
├── calibration/
├── dataset_raw/
├── src/
├── results/
├── requirements.txt
└── README.md# RET503-Computer-Vision-and-Deep-Learning
Tugas
