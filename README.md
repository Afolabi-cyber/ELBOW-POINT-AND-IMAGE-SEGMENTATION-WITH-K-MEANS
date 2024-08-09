# Image Color Segmentation using K-Means Clustering with Elbow Point Method

## Overview

This project demonstrates the application of K-Means clustering for image color segmentation, with a specific focus on determining the optimal number of clusters (k-value) using the elbow point method. The project uses a sample image of a flower to segment the image into distinct color regions based on the K-Means algorithm.

## Key Concepts

### K-Means Clustering

K-Means is an unsupervised machine learning algorithm that groups data points into `k` clusters, where each data point belongs to the cluster with the nearest mean. The algorithm aims to minimize the variance within each cluster.

### Elbow Point Method

Determining the optimal `k` value is crucial for effective clustering. The elbow point method is a heuristic used to find the optimal number of clusters. It involves plotting the within-cluster sum of squares (WCSS) against the number of clusters. The point where the reduction in WCSS starts to slow down, forming an "elbow," is considered the optimal `k` value.

### Image Color Segmentation

Image segmentation is the process of partitioning an image into multiple segments (sets of pixels). K-Means clustering can be applied to segment the image based on color. By clustering the pixel colors into `k` clusters, the image is effectively segmented into `k` dominant colors.

## Workflow

1. **Load the Image**: The flower image is loaded into the workspace.
2. **Preprocess the Image**: The image is reshaped into a 2D array of pixels, and the color values are normalized.
3. **Determine Optimal `k`**: The elbow point method is applied to determine the optimal number of clusters for color segmentation.
4. **Apply K-Means Clustering**: The K-Means algorithm is run with the optimal `k` to segment the image into `k` color regions.
5. **Reconstruct and Display the Segmented Image**: The clustered pixels are mapped back to the original image dimensions, and the segmented image is displayed.

## Requirements

- Python 3.x
- NumPy
- OpenCV
- Matplotlib
- scikit-learn

## How to Run

1. Install the required libraries:

   ```bash
   pip install numpy opencv-python matplotlib scikit-learn
