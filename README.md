# Image Processing Readme

This repository contains a Python script for image processing using the OpenCV and scikit-image libraries. The script performs various image processing tasks, such as thresholding, filtering, and contour extraction. Below is an overview of the functionalities implemented in the script.

## Table of Contents

- [Requirements](#requirements)
- [Usage](#usage)
- [Functions](#functions)
  - [Thresholding](#thresholding)
  - [Filtering](#filtering)
  - [K-Means Clustering](#k-means-clustering)
  - [Contour Extraction](#contour-extraction)

## Requirements

Make sure you have the following libraries installed before running the script:

- cv2
- matplotlib
- numpy
- skimage

You can install these dependencies using the following command:

```bash
pip install opencv-python matplotlib numpy scikit-image
```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repository.git
   ```

2. Navigate to the repository directory:

   ```bash
   cd your-repository
   ```

3. Run the script:

   ```bash
   python image_processing_script.py
   ```

## Functions

### Thresholding

In the script, thresholding is applied using Otsu's method. The image is loaded, converted to grayscale, and then thresholded to create a binary image.

### Filtering

A function `filter_image` is defined to filter an image based on a given mask. The script uses this function to filter the loaded image using the binary image obtained from the thresholding step.

### K-Means Clustering

The script demonstrates K-Means clustering on the input image. The image is reshaped and converted into a 3D array, and then K-Means clustering is applied to segment the image into k clusters.

### Contour Extraction

The script performs contour extraction on the input image. It converts the image to grayscale, applies thresholding, and detects contours using the Canny edge detector. The largest contour is then used to create a mask, and the original image is masked to extract the region of interest.

Feel free to explore and modify the script to suit your image processing needs!
