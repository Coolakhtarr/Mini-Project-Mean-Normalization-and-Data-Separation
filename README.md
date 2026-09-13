# Mean Normalization and Data Separation

This mini-project explores essential data preprocessing techniques used in machine learning with NumPy. It demonstrates how to normalize feature data and organize it into training, cross-validation, and test sets for more reliable model development and evaluation.

## Overview
Preparing data is a critical step in any machine learning workflow. In this notebook, the dataset is first normalized to make feature values more comparable, then randomly separated into distinct subsets for training, validation, and testing. This process helps reduce bias from row ordering and supports better model assessment.

## What the project demonstrates
- Working with NumPy arrays for data preprocessing
- Applying mean normalization to feature data
- Generating randomized row indices for unbiased selection
- Using indexing and slicing to separate datasets
- Organizing data into training, cross-validation, and test sets

## Code walkthrough

### 1. Dataset setup
The notebook begins with a dataset stored as a NumPy array. This serves as the original feature matrix before any preprocessing is applied.

### 2. Mean normalization
The feature values are normalized to create a new array, `X_norm`. This step helps center the data and improves consistency across features, which is often useful before training machine learning models.

### 3. Randomized row selection
A separate array of row indices is created and randomized. Instead of splitting the dataset in its original order, the notebook uses these shuffled indices to select rows more fairly.

### 4. Split boundary calculation
The code calculates cutoff points based on percentages of the dataset size:
- 60% of the rows for training
- 20% of the rows for cross-validation
- 20% of the rows for testing

These boundaries are stored as integer positions and used to divide the shuffled row indices.

### 5. Data separation
Using NumPy indexing, the normalized dataset is split into:
- `X_train`
- `X_crossVal`
- `X_test`

Each subset contains a different group of rows while preserving all feature columns.

## Tools used
- Python
- NumPy
- Jupyter Notebook

## File included
- `Mean Normalization and Data Separation.ipynb`

## How to run
1. Open Jupyter Notebook using Anaconda Navigator or Anaconda Prompt
2. Navigate to the project folder
3. Launch and open `Mean Normalization and Data Separation.ipynb`

## Learning outcome
This project strengthens understanding of foundational preprocessing concepts in machine learning, especially normalization, randomized selection, and structured dataset splitting using NumPy.
