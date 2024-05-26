# PCA-Package

## Overview

This PCA (Principal Component Analysis) package calculates the PCA of a data frame and provides useful visualizations such as individual contributions, correlation circles, and inertia information.

Through this project, I honed my skills in using `numpy` and `matplotlib` to generate PCA visualizations. Additionally, I reverse-engineered the PCA class from `scikit-learn` to better understand its inner workings and build my own version from scratch.

## Features

- **Data Scaling and Centering**
  - Centering adjusts the mean of each variable to zero.
  - Reducing (standardizing) the data to unit variance.
- **PCA Calculation**
  - Computes eigenvalues and eigenvectors of the covariance matrix.
  - Projects data onto principal components.
- **Visualizations**
  - Scatter plot of individuals in 2D or 3D.
  - Correlation circle for variable relationships.
  - Scree plot of eigenvalues.
  - Individual contributions to principal components.

# Documentation

## PCA Class

### Methods

- **`validate_boolean(self, value, name)`**:
  Validates if a value is a boolean.

- **`scale_center(self, matrix)`**:
  Centers the data by subtracting the mean.

- **`scale_center_reduce(self, matrix)`**:
  Reduces the data by dividing by the standard deviation.

- **`fit(self, dimension)`**:
  Computes eigenvalues and eigenvectors of the covariance matrix.

- **`transform(self)`**:
  Projects the data onto the principal components.

- **`fit_transform(self, matrix, dimension)`**:
  Scales, centers, reduces, fits, and transforms the data.

- **`get_property(self)`**:
  Returns eigenvalues, eigenvectors, principal components, and the scaled data matrix.

- **`plot_individuals(self)`**:
  Plots a scatter plot of individuals in 2D or 3D space.

- **`plot_cercle_correlation(self, colors, variables)`**:
  Plots a correlation circle for variable relationships.

- **`plot_inertie_information(self)`**:
  Displays the scree plot of eigenvalues.

- **`contribution_individuelle(self)`**:
  Calculates the contribution of each individual to the principal components.

- **`plot_contribution(self)`**:
  Plots the individual contributions to the principal components.

