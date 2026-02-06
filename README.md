# Face Recognition using Eigenfaces (SVD-Based Method)

Eigenvalue-based face recognition using Singular Value Decomposition (SVD) implemented in MATLAB. The system recognizes faces by comparing eigenvalue feature vectors using Euclidean distance.

---

## Table of Contents
- [Overview](#overview)
- [Objectives](#objectives)
- [Methodology](#methodology)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Output](#output)
- [Future Improvements](#future-improvements)

---

## Overview

This project implements a face recognition system using eigenvalue-based
feature extraction derived from Singular Value Decomposition (SVD).
Facial images are converted into mathematical representations, and
recognition is performed by comparing eigenvalue feature vectors.

Each face image is converted to grayscale, resized to a fixed dimension,
and decomposed using SVD. The singular values represent dominant facial
features and are used for recognition. A test image is matched with the
dataset using Euclidean distance to determine the closest face.

This project demonstrates the application of linear algebra concepts such
as eigenvalues, matrix decomposition, and dimensionality reduction in
computer vision.

---

## Objectives

- Implement face recognition using eigenvalues
- Apply SVD for feature extraction
- Reduce image dimensionality
- Identify closest matching face from dataset

---

## Methodology

1. Load images from dataset.
2. Convert images to grayscale.
3. Resize images to fixed size (100 × 100).
4. Apply Singular Value Decomposition (SVD).
5. Extract singular values as feature vectors.
6. Store eigenvalue vectors.
7. Process test image similarly.
8. Compute Euclidean distance.
9. Select minimum distance as recognized face.

---

## Project Structure


