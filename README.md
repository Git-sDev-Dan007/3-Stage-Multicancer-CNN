# 3Stage: Multi-Cancer Classification using Histopathological Images

This repository contains a deep learning-based three-stage pipeline for multi-class cancer detection and classification using histopathological image data. The system identifies whether an image is cancerous, classifies the organ type, and further predicts the specific cancer subtype across 26 categories.

## 🚀 Project Overview

- **Stage 1**: Binary classification (Cancerous vs Non-Cancerous)  
- **Stage 2**: Organ-level classification (8 major cancer types)  
- **Stage 3**: Subtype-level classification (26 detailed subtypes)

Each stage is powered by a custom CNN model built using PyTorch, trained independently with class weighting, dropout, and data augmentation. Grad-CAM visualizations are integrated at every stage for explainability.

## 📊 Key Features

- ✅ Three-stage modular deep learning pipeline  
- ✅ Achieved up to 98% accuracy on organ classification  
- ✅ Grad-CAM heatmaps for transparent model interpretation  
- ✅ Handles class imbalance with weighted loss and augmentation  
- ✅ Scalable architecture suitable for clinical deployment

## 🗂️ Dataset

- 130,000 histopathological images  
- 8 major cancer types  
- 26 subtypes  
- Balanced per class (5,000 samples each)

> **Note**: Dataset not included due to size. Refer to [Kaggle Source](#) or modify the directory paths as needed.

## 📁 Folder Structure
├── stage1_binary_classifier.pth
├── stage2_organ_classifier.pth
├── stage3_subtype_classifier.pth
├── pipeline/
│ ├── preprocess.py
│ ├── model.py
│ ├── gradcam.py
│ └── run_pipeline.py
├── utils/
│ └── visualize.py
└── README.md

Project WorkFlow:

![Project Flowchart](https://github.com/user-attachments/assets/dc478870-adf2-4e8c-8098-d48b205dd0d4)

Time per Stage analysis:
![Time per Stage](https://github.com/user-attachments/assets/4079b708-9e14-4b8c-8f1e-cbeeb073d594)


Cancerous Prediction:
![Cancerous Output](https://github.com/user-attachments/assets/2676d155-e770-4f00-b9c9-5e94b734e0f5)

Non Cancerous Prediction:
![Non Cancerous Output](https://github.com/user-attachments/assets/8edfa46b-dd75-46e0-92bf-c1131aed3d41)

## 🧠 Future Work

- Integration with clinical metadata or genomic features  
- External validation on real-world patient datasets  
