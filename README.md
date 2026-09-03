# Rice Leaf Disease Detection and Classification

An end-to-end Computer Vision project designed to detect and classify common diseases in rice crops using deep learning techniques. This project aims to support early threat detection in precision agriculture to help minimize crop damage and improve yield quality.

---

## Table of Contents
* [Project Overview](#project-overview)
* [Dataset Description](#dataset-description)
* [Repository Structure](#repository-structure)
* [Technical Architecture & Workflow](#technical-architecture--workflow)
* [Installation & Setup](#installation--setup)
* [Usage Instructions](#usage-instructions)
* [Results & Evaluation](#results--evaluation)
* [Future Scope](#future-scope)
* [License](#license)

---

## Project Overview
Rice is a primary staple food for over half of the world's population. However, crop diseases severely affect production efficiency. Manual diagnosis is time-consuming, subjective, and prone to human error.

This project implements an automated image classification pipeline using Convolutional Neural Networks (CNN) / Transfer Learning models to classify rice leaf images into three distinct disease categories:
1. **Bacterial Leaf Blight** (*Xanthomonas oryzae*)
2. **Brown Spot** (*Cochliobolus miyabeanus*)
3. **Leaf Smut** (*Entyloma oryzae*)

---

## Dataset Description
The dataset contains high-resolution RGB images of rice leaves categorized by disease type. 

* **Source Archive**: `PRCP-1001-RiceLeaf.zip`
* **Target Classes**:
  * `Bacterial leaf blight`
  * `Brown spot`
  * `Leaf smut`
* **Preprocessing Applied**:
  * Image Resizing (e.g., 224x224 / 256x256 pixels)
  * Pixel Normalization (0–1 scaling or standardized ImageNet statistics)
  * Data Augmentation (Random rotations, flips, brightness adjustments) to prevent overfitting.

> **Note**: The raw dataset files are excluded from this repository via `.gitignore` to keep the codebase light. Follow the setup instructions below to prepare local data.

---

## Repository Structure

```text
├── .gitignore               # Excludes large archives, datasets, and checkpoint files
├── README.md                # Detailed project documentation
├── requirements.txt         # Project dependencies and environment specs
└── RiceLeaf.ipynb           # Main Jupyter Notebook containing EDA, preprocessing, and training
