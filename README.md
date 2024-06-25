# Camera-Calibration-with-Images

# Camera Calibration and Distance Measurement

This repository contains the implementation of a camera calibration and distance measurement project using OpenCV. The primary goal is to perform intrinsic calibration of a monocular camera using a checkerboard pattern to accurately compute the camera's distance from the checkerboard during various poses.

## Introduction

Camera calibration is crucial for accurate metric measurements in computer vision tasks. This project uses a checkerboard because of its high contrast pattern, making it easy to detect and use for extracting precise camera parameters. By understanding these parameters, we can compute the camera's distance from the checkerboard, which is essential for applications in 3D reconstruction, robotics, and augmented reality.

## Project Overview

- **Calibration Process**: The camera calibration is performed using OpenCV's calibration functions. The process involves capturing several images of a checkerboard in different positions and orientations.
- **Distance Computation**: After calibration, the project computes the distance from the camera to the checkerboard using the derived camera parameters.
- **Pose Estimation**: Additionally, the pose (orientation and position) of the checkerboard is estimated relative to the camera.

## Key Features

- **Automated Corner Detection**: Utilizes `cv2.findChessboardCorners` for accurate corner detection in calibration images.
- **Camera Calibration**: Employs `cv2.calibrateCamera` to determine the camera matrix and distortion coefficients.
- **Pose Estimation**: Uses `cv2.solvePnP` to find the rotation and translation vectors describing the checkerboard's pose.
- **Distance Measurement**: The distance from the camera to the checkerboard is computed and displayed for each image.

## Setup and Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/camera-calibration.git
2. **Setup the Google Colab Notebook:**
   ```bash
   Open the notebook link provided in the project: Google Colab Notebook.
   Use "Save a Copy in Drive" to create a personal editable version.
   Upload calibration images to the images folder in the notebook environment.
3. **Run the Notebook:**
  ```bash
  Execute the notebook cells step-by-step to perform camera calibration and distance measurements.
  View and analyze the outputs directly in the notebook.
