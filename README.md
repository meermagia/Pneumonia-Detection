# Pneumonia Detection Using Image Pre-processing Techniques

## Overview
This project implements a structured image preprocessing pipeline designed to enhance chest X-ray images for robust pneumonia detection. By employing a diverse set of image enhancement and feature extraction techniques, this pipeline improves visibility, texture clarity, and edge sharpness, serving as a foundation for downstream machine learning models.

## Authors
* **Nilay Jain**
* **Karan Lokhande**
* **Yuvan Jain**
* **Meer Magia**

*Dept. of Artificial Intelligence, NMIMS Mukesh Patel School of Technology Management and Engineering*.

## Methodology
The pipeline processes raw X-ray images through the following 13 steps to generate a "Final Fusion" enhanced image:

1.  **Grayscale Conversion:** Basic image formatting.
2.  **Gaussian Blur:** Denoising the image.
3.  **Histogram Equalization:** Global contrast adjustment.
4.  **CLAHE:** Contrast Limited Adaptive Histogram Equalization for local contrast.
5.  **Unsharp Masking:** Sharpening the image details.
6.  **Canny Edge Detection:** Identifying structural edges.
7.  **Wavelet Transform (Haar):** Extracting frequency details.
8.  **Median Blurring:** Further noise reduction.
9.  **Sobel Operator:** Gradient-based edge extraction.
10. **Morphological Closing:** Closing small holes in foreground objects.
11. **Morphological Erosion:** Refining object boundaries.
12. **Final Fusion:** Weighted combination of Unsharp Masking and Wavelet details, with edges highlighted.
13. **Color Mapping:** Applying a blue-based colormap (COLORMAP_OCEAN) for visual interpretability.

## Installation
To run this project, install the required dependencies:

```bash
pip install -r requirements.txt

