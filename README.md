# Image Processing and Computer Vision Project

This repository contains two computer vision tasks:

1. **Book Detection on Shelves** – using classical image processing and feature-based techniques.  
2. **Oxford-IIIT Pet Dataset Classification** – building and fine-tuning deep learning models for pet breed classification.

---

## Table of Contents

- [Project Overview](#project-overview)  
- [Task 1: Book Detection on Shelves](#task-1-book-detection-on-shelves)  
- [Task 2: Oxford-IIIT Pet Dataset Classification](#task-2-oxford-iiit-pet-dataset-classification)  
- [License](#license)

---

## Project Overview

This project explores two key areas of computer vision:

1. **Detection of objects (books) in cluttered environments** using feature-based classical techniques.  
2. **Image classification and model fine-tuning** on a benchmark dataset (Oxford-IIIT Pet Dataset).

---

## Task 1: Book Detection on Shelves

### Objective
Detect and localize multiple books on shelves using classical feature-based computer vision techniques.

### Pipeline
The detection pipeline includes:

1. **CLAHE (Contrast Limited Adaptive Histogram Equalization)** – enhances image contrast to improve feature detection.  
2. **Feature Extraction with RootSIFT Descriptors** – detect keypoints and compute RootSIFT descriptors for robust matching.  
3. **Feature Matching with FLANN-based Matcher** – efficiently match descriptors between book templates and shelf images.  
4. **Geometric Verification with RANSAC** – filter matches to retain geometrically consistent correspondences and estimate book locations.  
5. **Keypoint Filtering and Multi-instance Detection** – detect multiple instances of the same book by iteratively refining matches.

### Dependencies
- Python 3.x  
- OpenCV (`cv2`)  
- NumPy  

---

## Task 2: Oxford-IIIT Pet Dataset Classification

### Objective
Train and fine-tune deep learning models to classify pet breeds in the Oxford-IIIT Pet Dataset.

### Approach
1. Preprocess images (resizing, normalization, augmentation).  
2. Split dataset into training, validation, and test sets.  
3. Use pre-trained CNN architectures for transfer learning (e.g., ResNet, EfficientNet).  
4. Fine-tune models for optimal performance on pet breed classification.  
5. Evaluate models using accuracy, F1-score, and confusion matrices.

### Dependencies
- Python 3.x  
- PyTorch or TensorFlow  
- torchvision or tf.keras  
- NumPy  
- Matplotlib  

---

## License
This project is released under the MIT License. You are free to use, modify, and distribute the code for educational purposes.
