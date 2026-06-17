# 🌿 Plant Leaf Dataset Analysis & CNN Training Pipeline

## 📌 Project Overview

This project focuses on deep learning model preparation for plant leaf disease classification using a structured workflow:

- 📊 Dataset analysis and visualization
- 🔄 Data augmentation to balance classes
- 🧠 Image transformation for feature understanding
- 🤖 Training a CNN model for classification

The goal is to deeply understand the dataset and improve model performance through preprocessing and augmentation techniques.

## 📊 1. Dataset Analysis
### 🧩 Objective

The first step is to analyze the dataset structure and distribution of images across classes.

The dataset is organized in a hierarchical directory format:

-   ./Apple
-   ./Apple/apple_healthy
-   ./Apple/apple_apple_scab
-   ./Apple/apple_black_rot
-   ./Apple/apple_cedar_apple_rust
## 🛠️ Tool: Distribution.[extension]
### 📥 Input

A directory containing subfolders of plant classes:

./Distribution.[extension] ./Apple
### ⚙️ Functionality

The program must:

- Traverse all subdirectories
- Count images per class
- Extract plant/disease names from folder structure
- Analyze dataset distribution
### 📊 Output

For each plant type:

- Bar chart showing number of images per class
- Pie chart showing percentage distribution

- Each chart must be automatically labeled using folder names.

## 🎯 Goal
- Identify dataset imbalance
- Understand class distribution
- Prepare for augmentation step
## 🔄 2. Data Augmentation
### 📌 Problem

The dataset is imbalanced, meaning some classes have more images than others.

## 🧠 Objective

Balance dataset using image augmentation techniques.

## 🛠️ Tool: Augmentation.[extension]
### 📥 Input

A single image:

- ./Augmentation.[extension] ./Apple/apple_healthy/image(1).JPG
## ⚙️ Augmentation Techniques

Each image must generate 6 augmented versions:

- 🔄 Flip
- 🔁 Rotate
- 📐 Skew
- ✂️ Shear
- 🔲 Crop
- 🌫️ Distortion
## 💾 Output

All augmented images must be saved in the same directory:

- image(1)_Flip.JPG
- image(1)_Rotate.JPG
- image(1)_Skew.JPG
- image(1)_Shear.JPG
- image(1)_Crop.JPG
- image(1)_Distortion.JPG
## 🎯 Goal
- Balance dataset classes
- Increase training diversity
- Improve CNN generalization
## 🖼️ 3. Image Transformation & Feature Extraction
### 📌 Objective

Apply image processing techniques to extract meaningful features from leaf images.

This helps understand:

- Disease patterns
- Leaf structures
- Visual anomalies
## 🛠️ Tool: Transformation.[extension]
### 📥 Input
- ./Transformation.[extension] ./Apple/apple_healthy/image(1).JPG
## ⚙️ Required Transformations

At least 6 transformations must be displayed:

1. Original Image

- Baseline input image

2. Gaussian Blur

- Reduces noise and smooths image

3. Masking

- Isolates leaf regions from background

4. ROI Extraction

- Detects regions of interest (leaf areas)

5. Object Analysis

- Extracts shape and structural features

6. Pseudo-Landmarks

- Identifies key structural points of the leaf

## 🎯 Goal
- Understand visual features of plant leaves
- Extract useful patterns for CNN training
- Improve preprocessing pipeline
## 🧠 Final Goal of This Pipeline

This project builds a complete preprocessing and analysis system for plant leaf disease detection using deep learning:

Dataset Analysis → Data Balancing → Image Transformation → CNN Training

## 👩‍💻 Author

### Fatima Ezzahra Ouaourikt || Chaimaa Lyamani
Software Engineering Student • Machine Learning Enthusiast • Computer Vision Learner
