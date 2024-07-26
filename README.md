# Banknote Authentication Using kNN Model

A k-nearest neighbors (kNN) model implemented to classify banknotes as authentic or counterfiet based on features extracted from the images of banknotes.

## Overview

This project demonstrates the implementation of a k-nearest neighbors (kNN) model to classify banknotes. The dataset used is the Banknote Authentication dataset. The kNN algorithm is implemented from scratch and also using the `sklearn` library for comparison. The project invloves data preprocessing, model training, evaluation, and visualization.

## Table of Contents

- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Implementation](#implementation)
  - [From Scratch](#from-scratch)
  - [Using sklearn](#using-sklearn)
- [Results](#results)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Resources](#resources)
- [Contributing](#contributing)

## Project Structure

- `kNN.ipynb`: Jupyter Notebook containing the implementation of the kNN model from scratch and using `sklearn`.
- `data_banknote_authentication.txt`: Dataset file.
- `README.md`: Project documentation.

## Dataset

The data used is `data_banknote_authentication.txt`, which contains features extracted from images of banknotes using wavelet transform tools. The columns in the dataset are:
- `Variance of Wavelet Transformed image` (continous)
- `Skewness of Wavelet Transformed image` (continuous)
- `Kurtosis of Wavelet Transformed image` (continuous)
- `Entropy of image` (continuous)
- `Class` (integer): 0 for authentic, 1 for counterfeit

## Implementation

### From Scratch 

The k-nearest neighbors (kNN) model is first implemented from scratch using Python. The process involves:
1. Calculating the Euclidean distance between the test data point and all training data points.
2. Sorting the distances and selecting the k-nearest neighbors.
3. Performing majority voting to classify the test data point.

### Using sklearn

The `sklearn` library is then utilized to perform k-nearest neighbors classification on the same dataset. The steps include:
1. Importing the `KNeighborsClassifier` model from `sklearn`.
2. Fitting the model to the training dataset.
3. Making predictions and comparing them with the from-scratch implementation.

## Results

The results section compares the predictions made by the from-scratch implementation and the `sklearn` model, highlighting any differences and similarities. It includes performance metrics such as accuracy, precision, recall, and F1-score.

## Dependencies

- Python 3.x
- Jupyter Notebook
- numpy
- pandas
- matplotlib
- sklearn

Install the dependencies using:
```bash
pip install numpy pandas matplotlib sklearn jupyter
```

## Usage 

1. Clone the repository:

```bash
git clone https://github.com/yourusername/k-nearest.git
```

2. Navigate to project directory:

```bash
cd k-nearest
```

3. Open the Jupyter notebook:

```bash
jupyter notebook kNN.ipynb
```