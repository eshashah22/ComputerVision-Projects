# Stereo Depth Estimation

## Introduction
This project implements a stereo vision system that estimates depth from two camera views.

## Pipeline Overview
1. **Image Rectification**  
    - Compute transformation between right and left camera views
    - Apply homography to align epipolar lines horizontally
   
2. **Disparity Computation**  
    - Use SSD to match patches
    - Perform left-right consistency check to filter unreliable matches
   
3. **Depth Reconstruction**  
    - Convert disparity to depth using baseline and focal length
    - Back-project pixels to 3D space using camera parameters
