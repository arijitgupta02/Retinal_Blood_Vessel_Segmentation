# Retinal Blood Vessel Segmentation using Attention Residual U-Net

## Overview

This project presents a deep learning based approach for automated retinal blood vessel segmentation using an Attention Residual U-Net architecture implemented in PyTorch. The model is designed to accurately extract fine vascular structures from retinal fundus images, which can assist in the early diagnosis of ophthalmic diseases such as Diabetic Retinopathy, Glaucoma, Hypertension, and Cardiovascular Disorders.

The project includes image preprocessing, CLAHE enhancement, vessel segmentation, performance evaluation, ROC analysis, and visualization of segmentation outputs using the DRIVE retinal dataset.

---

## Objectives

- Perform retinal vessel segmentation from fundus images
- Improve vessel visibility using preprocessing techniques
- Develop an Attention Residual U-Net model for precise segmentation
- Evaluate segmentation performance using medical imaging metrics
- Visualize prediction outputs and segmentation quality

---

## Dataset

Dataset Used:
- DRIVE (Digital Retinal Images for Vessel Extraction)

Dataset contains:
- Retinal fundus images
- Ground truth vessel masks
- Training and testing samples for segmentation tasks

---

## Key Features

- Retinal image preprocessing using Green Channel Extraction
- CLAHE based contrast enhancement
- Binary vessel mask generation
- Attention Residual U-Net implementation
- Deep learning based vessel segmentation
- Prediction visualization
- ROC Curve and segmentation evaluation
- Medical image analysis workflow using PyTorch

---

## Technologies Used

- Python
- PyTorch
- NumPy
- OpenCV
- Matplotlib
- Scikit-learn
- Albumentations

---

## Project Workflow

1. Data Loading
2. Image Preprocessing
3. Green Channel Extraction
4. CLAHE Enhancement
5. Ground Truth Mask Preparation
6. Data Augmentation
7. Model Architecture Design
8. Model Training
9. Vessel Segmentation Prediction
10. Performance Evaluation
11. Visualization and Analysis

---

## Model Architecture

The project uses an Attention Residual U-Net architecture that combines:
- Residual Connections for improved gradient flow
- Attention Gates for focusing on important vessel regions
- Encoder-Decoder segmentation framework for pixel-level prediction

This architecture improves segmentation accuracy for thin and low-contrast retinal vessels.

---

## Image Preprocessing

The preprocessing pipeline includes:
- Green channel extraction from RGB retinal images
- Contrast enhancement using CLAHE
- Image normalization
- Binary mask preparation

These techniques improve vessel visibility and segmentation quality.

---

## Results

The model successfully segments retinal blood vessels with high visual similarity to ground truth masks.

The project demonstrates:
- Accurate vessel extraction
- Preservation of thin vascular structures
- Improved segmentation performance on low-contrast retinal images
- Strong segmentation quality on retinal fundus images

---

## Sample Outputs

### Original Image and Ground Truth Mask

![Ground Truth](images%20%26%20Visual%20Output/ground_truth_mask.png)

---

### Preprocessed Retinal Image

![Preprocessing](images%20%26%20Visual%20Output/dataset_preprocessing.png)

---

### Segmentation Prediction Result 1

![Prediction 1](images%20%26%20Visual%20Output/segmentation_prediction_1.png)

---

### Segmentation Prediction Result 2

![Prediction 2](images%20%26%20Visual%20Output/segmentation_prediction_2.png)

---

### ROC Curve

![ROC Curve](images%20%26%20Visual%20Output/roc_curve.png)

---

## Project Structure

```text
retinal-blood-vessel-segmentation/
│
├── retinal_image_segmentation.ipynb
├── README.md
├── requirements.txt
├── DRIVE/
│   ├── train/
│   │   ├── 1st_manual/
│   │   ├── images/
│   │   └── masks/
│   │
│   └── test/
│       ├── 1st_manual/
│       ├── images/
│       └── masks/
│
└── images & Visual Output/
    ├── dataset_preprocessing.png
    ├── ground_truth_mask.png
    ├── segmentation_prediction_1.png
    ├── segmentation_prediction_2.png
    └── roc_curve.png
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/retinal-blood-vessel-segmentation.git
```

Move into the project directory:

```bash
cd retinal-blood-vessel-segmentation
```

Install required dependencies:

```bash
pip install -r requirements.txt
```

---

## Requirements

```txt
torch
torchvision
numpy
opencv-python
matplotlib
scikit-learn
albumentations
```

---

## Run the Project

Open the notebook:

```bash
jupyter notebook
```

Run:

```text
segmentation_retinal_image.ipynb
```

---

## Applications

- Diabetic Retinopathy Detection
- Ophthalmic Disease Analysis
- Medical Image Segmentation
- Clinical Decision Support Systems
- Automated Retinal Screening

---

## Future Improvements

- Integration with Transformer based segmentation models
- Real-time retinal vessel segmentation
- Cross-dataset generalization
- Explainable AI for medical imaging
- Deployment as a web application

---

## Author

Arijit Gupta
