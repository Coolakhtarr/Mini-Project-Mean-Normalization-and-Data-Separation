# Mean Normalization and Data Separation

This mini-project demonstrates how to preprocess data with NumPy for machine learning. The notebook focuses on mean normalization and splitting data into training, cross-validation, and test sets.

## Project overview
The code is organized around a simple preprocessing workflow:
1. Start with the original dataset
2. Normalize the feature values
3. Shuffle the row indices
4. Calculate split points
5. Separate the data into training, cross-validation, and test sets

## Code stages

### 1. Create or load the dataset
The project begins with a NumPy array containing the original feature data. This array represents the full dataset before preprocessing.

### 2. Apply mean normalization
The dataset is normalized so that feature values are centered and scaled more consistently. This helps prepare the data for machine learning tasks.

### 3. Generate randomized row indices
A separate array of row indices is created and shuffled. These indices are used to select rows in random order instead of relying on the original arrangement of the dataset.

### 4. Calculate split boundaries
The code computes cutoff points for 60% and 80% of the dataset. These values define how the rows will be divided:
- First 60% for training
- Next 20% for cross-validation
- Final 20% for testing

### 5. Split the normalized dataset
Using NumPy indexing and slicing, the normalized dataset is separated into:
- `X_train`
- `X_crossVal`
- `X_test`

Each split keeps all columns while selecting different groups of rows.

## Tools used
- Python
- NumPy
- Jupyter Notebook

## File
- `Mean Normalization and Data Separation.ipynb`

## How to run
1. Open Jupyter Notebook through Anaconda Navigator or Anaconda Prompt
2. Navigate to the project folder
3. Open `Mean Normalization and Data Separation.ipynb`

## Purpose
This project is intended as practice for understanding essential data preprocessing techniques used before training machine learning models.
