# Lane Detection Project

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Features](#features)
- [Theory](#theory)
  - [Lane Detection Algorithm](#lane-detection-algorithm)
  - [Preprocessing](#preprocessing)
  - [Canny Edge Detection](#canny-edge-detection)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)

## Overview

Lane detection is a critical aspect of autonomous navigation systems for vehicles and robotics. This project offers a comprehensive lane detection solution using computer vision techniques and OpenCV. It aims to provide a robust lane detection algorithm that can be integrated into various applications.

## Project Structure

The project structure is organized as follows:

- `Lane_Detection.ipynb`: Jupyter Notebook with the main lane detection code.
- `images/`: Directory containing sample images for testing and development.
- `README.md`: This documentation file.

## Features

- Preprocessing of input images to enhance lane visibility.
- Canny edge detection for identifying lane edges.
- Definition of a region of interest (ROI) for focused lane detection.
- Visualization of lane detection results on input images.

## Theory

### Lane Detection Algorithm

The lane detection algorithm follows these main steps:

1. **Preprocessing**: Enhance the input image to improve lane visibility.
2. **Canny Edge Detection**: Detect edges in the preprocessed image.
3. **Region of Interest (ROI) Masking**: Define an ROI to focus on the lane area.
4. **Hough Transform**: Detect lines in the ROI.
5. **Lane Fitting**: Fit the detected lines to identify left and right lanes.
6. **Visualization**: Display the lane detection results on the original image.

### Preprocessing

The preprocessing step includes techniques such as gamma correction to enhance image brightness and improve lane visibility. Gamma correction is applied using the formula:gamma_corrected = (image / 255.0) ** gamma * 255


### Canny Edge Detection

Canny edge detection is employed to identify edges in the preprocessed image. It uses a Gaussian filter for noise reduction and then applies gradient calculations to detect edges.

## Getting Started

Follow these instructions to set up the project on your local machine.

### Prerequisites

Ensure you have the following dependencies installed:

- Python (3.6+)
- OpenCV
- NumPy
- Matplotlib (for visualization)

You can install the required packages using `pip`:

```bash
pip install opencv-python numpy matplotlib


