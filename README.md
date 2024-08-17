# AWS Nano Degree Project 1: Dog Image Classifier

## Overview

This project focuses on evaluating image classification algorithms to determine their effectiveness in categorizing images as "dogs" or "not dogs" and further classifying the breed of dogs. We compare the performance of different Convolutional Neural Network (CNN) models—ResNet, AlexNet, and VGG—based on accuracy and computational efficiency.

## Objectives

### Classify Pet Images
- Identify which images are of dogs, even if the breed is not correctly classified.
- For images identified as dogs, classify their breed accurately.

### Evaluate CNN Models
- Determine which CNN model architecture (ResNet, AlexNet, VGG) performs best in achieving the above objectives.

### Assess Computational Efficiency
- Measure the runtime of each algorithm to understand the trade-off between accuracy and computational resources.
- Evaluate if a less accurate model might be a suitable alternative based on performance and time constraints.

## Project Outline

### Setup and Initialization
- **Timing:** Use the `time` module to measure the runtime of each algorithm.
- **Inputs:** Gather program inputs from user-provided command line arguments.

### Label Creation
- **Pet Images:** Generate labels for pet images using their filenames and store these labels in a suitable data structure (e.g., dictionary).

### Classification and Comparison
- **Classifier Labels:** Use the image classification algorithm to generate labels and compare these with the pet image labels.
- **Data Structure:** Store pet image labels, classifier labels, and their comparisons in a complex data structure (e.g., dictionary of lists).

### Classify as "Dogs" or "Not Dogs"
- Use a reference file (`dognames.txt`) to classify images as "dogs" or "not dogs."
- Update the data structure to reflect these classifications.

### Results Calculation and Output
- Analyze the results based on the labels and their classifications to evaluate the algorithm's performance.
- Print the results for review and further analysis.

## How to Use

### Install Dependencies
Make sure you have all necessary Python packages installed. You may need libraries such as `numpy`, `scikit-learn`, and specific deep learning frameworks (e.g., TensorFlow or PyTorch).

### Run the Program
Execute the program using command line arguments to specify inputs such as image directories or model choices.

### Example Command

```bash
python classify_images.py --input_dir /path/to/images --model ResNet
