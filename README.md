# Sampling with SMOTE: Handling Class Imbalance

This repository contains a Jupyter Notebook, **`Sampling.ipynb`**, which demonstrates techniques for handling class imbalance in datasets using **SMOTE (Synthetic Minority Oversampling Technique)**. 

## Overview

Class imbalance is a common issue in machine learning, where one class significantly outnumbers others. This imbalance can lead to biased models. To address this, the notebook focuses on:
- Visualizing class distributions before and after resampling.
- Applying SMOTE to balance the dataset.
- Recombining features and target variables after resampling.

## Key Steps in the Notebook

1. **Dataset Preparation**  
   - The dataset is split into features (`X`) and the target variable (`y`).

2. **Class Distribution Analysis**  
   - Visualize the distribution of the target variable before resampling using `countplot`.

3. **Applying SMOTE**  
   - SMOTE is used to oversample the minority class, balancing the dataset.

4. **Class Distribution After Resampling**  
   - Post-SMOTE, the class distribution is visualized for comparison.

5. **Recombining the Dataset**  
   - Features and target variables are recombined into a single DataFrame for further use.

6. **Code Highlights**
   - Visualization using `seaborn` and `matplotlib`.
   - SMOTE application with `imblearn.over_sampling`.

## Requirements

To run the notebook, make sure the following dependencies are installed:
- Python 3.x
- Jupyter Notebook or JupyterLab
- Required libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn imbalanced-learn
  ```

## Visualizations

- **Before Resampling**: Bar charts to show the original class imbalance.
- **After Resampling**: Bar charts demonstrating the balanced dataset.


## Example Outputs

### Class Distribution (Before and After Resampling)

- Before Resampling:
  ![Original Class Distribution](path-to-image-before.png)

- After Resampling:
  ![Resampled Class Distribution](path-to-image-after.png)

### Sample of Resampled Dataset
| Feature 1 | Feature 2 | Feature 3 | Class |
|-----------|-----------|-----------|-------|
| 1.2       | 3.4       | 2.1       | 0     |
| 4.5       | 1.2       | 5.4       | 1     |
