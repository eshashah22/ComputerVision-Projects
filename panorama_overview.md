# Panorama Stitching

## Introduction
This project takes multiple overlapping images and creates a panoramic image by detecting features, matching them across images, and blending them together.

## Pipeline Overview
1. Corner detection
2. Adaptive Non-Maximal Suppression (ANMS) for even feature distribution
3. Feature description using patch-based vector descriptors
4. Feature matching across image pairs
5. RANSAC homography estimation
6. Image warping and blending
7. Stitching multiple consecutive images
