# Face Recognition Using Eigenvalues (SVD-Based Approach)

## Overview

This project presents a face recognition system implemented using **Singular Value Decomposition (SVD)** and eigenvalue-based feature extraction in MATLAB. The system identifies a person by comparing the eigenvalue representation of facial images instead of directly comparing pixel values.

Each face image is transformed into a compact mathematical representation using singular values, which capture the most important structural information of the face. Recognition is performed by measuring the Euclidean distance between eigenvalue vectors of the test image and the training dataset.

This project demonstrates the application of **linear algebra concepts such as eigenvalues, matrix decomposition, and dimensionality reduction** in computer vision.

---

## Objectives

- Implement a face recognition system using eigenvalue-based features.
- Apply Singular Value Decomposition (SVD) for feature extraction.
- Reduce image dimensionality while preserving important facial information.
- Recognize unknown faces using similarity measurement.
- Demonstrate practical applications of linear algebra in image processing.

---

## Methodology

The system follows the steps below:

### Image Acquisition
- Face images are loaded from a dataset folder.
- All images are assumed to be in `.jpg` format.

### Preprocessing
- Images are converted to grayscale.
- Images are resized to a fixed dimension (100 × 100).
- Images are converted to double precision for mathematical computation.

### Feature Extraction using SVD

Singular Value Decomposition is applied:

A = U S Vᵀ

Where:
- **U** and **V** contain orthogonal basis vectors.
- **S** contains singular values representing dominant facial features.

The diagonal elements of matrix **S** are extracted and stored as feature vectors.

### Testing Phase
- A new test image undergoes the same preprocessing steps.
- Its eigenvalues are computed using SVD.

### Face Matching
Euclidean distance is calculated between the test image eigenvalues and stored image eigenvalues:

d = √ Σ (xi − yi)²

The image with minimum distance is selected as the closest match.

---

## Key Concepts Used

- Singular Value Decomposition (SVD)
- Eigenvalues and Eigenvectors
- Linear Algebra
- Image Processing
- Feature Extraction
- Euclidean Distance Matching

---

## Technologies Used

- MATLAB
- Image Processing Toolbox
- Linear Algebra Methods

---

## Project Structure

