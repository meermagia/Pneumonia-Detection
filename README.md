# Pneumonia-Detection
Pneumonia Detection Using Image Pre-processing Techniques

Overview

This project implements a structured image preprocessing pipeline designed to enhance chest X-ray images for robust pneumonia detection. [cite_start]By employing a diverse set of image enhancement and feature extraction techniques, this pipeline improves visibility, texture clarity, and edge sharpness, serving as a foundation for downstream machine learning models[cite: 104, 120].

Authors

Nilay Jain
Karan Lokhande
Yuvan Jain
Meer Magia
[cite_start]Dept. of Artificial Intelligence, NMIMS Mukesh Patel School of Technology Management and Engineering[cite: 105, 108, 114, 116].

Methodology

The pipeline processes raw X-ray images through the following 13 steps to generate a "Final Fusion" enhanced image:

Grayscale Conversion: Basic image formatting.
Gaussian Blur: Denoising the image.
Histogram Equalization: Global contrast adjustment.
CLAHE: Contrast Limited Adaptive Histogram Equalization for local contrast.
Unsharp Masking: Sharpening the image details.
Canny Edge Detection: Identifying structural edges.
Wavelet Transform (Haar): Extracting frequency details.
Median Blurring: Further noise reduction.
Sobel Operator: Gradient-based edge extraction.
Morphological Closing: Closing small holes in foreground objects.
Morphological Erosion: Refining object boundaries.
Final Fusion: Weighted combination of Unsharp Masking and Wavelet details, with edges highlighted.
Color Mapping: Applying a blue-based colormap (COLORMAP_OCEAN) for visual interpretability.
Installation

To run this project, install the required dependencies:

pip install -r requirements.txt
