# fMRI Data Analysis and Classification

This project demonstrates the use of machine learning techniques to analyze and classify brain activation patterns from fMRI data. The primary goal is to identify and predict task-specific brain activation, focusing on two tasks: **Lips** and **Finger**.

## Project Overview

The project follows a pipeline that includes data preprocessing, statistical analysis, and machine learning classification. The analysis aims to:

- Explore brain activation patterns during specific tasks.
- Compare activation patterns across tasks.
- Build a classifier to predict task types based on voxel activation data.
- Evaluate the classifier's performance using various metrics.

## Key Components

### 1. **Data Preprocessing**
- Loading and validating neuroimaging data.
- Scaling the activation data to ensure proper numerical stability.
- Handling out-of-bounds indices during data extraction.

### 2. **Statistical Analysis**
- Exploring task-specific brain activation.
- Comparing brain activation patterns between different tasks using statistical tests.

### 3. **Machine Learning Classification**
- Built a **Random Forest** model to predict task types (Lips vs. Finger) based on voxel activation.
- Applied **Logistic Regression** for a baseline comparison.
- Used **cross-validation** to improve the model's performance.
- Evaluated model performance using metrics such as accuracy, precision, recall, and F1-score.

### 4. **Visualization**
- Visualized brain activation patterns on fMRI slices.
- Generated feature importance plots for the Random Forest model to interpret key contributing features.

## Getting Started

To run this project locally, follow these steps:

### Prerequisites
Ensure you have the following libraries installed in your R environment:
- `caret`
- `randomForest`
- `ggplot2`
- `dplyr`

```r
install.packages(c('caret', 'randomForest', 'ggplot2', 'dplyr'))
