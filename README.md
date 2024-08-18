# Project Overview

This project is a component of the AWS AI & ML scholarship program offered through Udacity. The goal is to develop a command-line application in Python that uses a pre-trained image classifier, trained on the ImageNet dataset, to determine if an image depicts a dog and, if so, identify the breed of the dog.

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


# Project Requirements:
This project analyzes pet images using a Convolutional Neural Network (CNN) classifier. It performs the following tasks:

* **Timing Measurement:** Tracks the execution time of the core logic using timing functions (Functionality implemented in Python).
* **Command-Line Arguments:** Accepts various arguments: (Functionality implemented in Python)
    * `--dir (default: pet_images/)`: Path to the directory containing pet images.
    * `--arch (default: vgg)`: Specifies the CNN architecture (e.g., VGG, ResNet, AlexNet).
    * `--dogfile (default: dognames.txt)`: File containing a list of recognized dog breeds.
* **File Filtering:** Excludes files beginning with a dot (e.g., `.DS_Store`) from processing (Functionality likely implemented in Python).
* **Dictionary Format:** Validates the format of dictionary keys and labels, retrieving up to 40 key-value pairs (e.g., `{'Poodle_07956.jpg': ['poodle'], 'fox_squirrel_01.jpg': ['fox squirrel'], ...}`). (Functionality likely implemented in Python).
* **Argument Passing:** Passes the `--dir` argument to the `check_images.py` script during the `get_pet_labels` function call (Functionality implemented in Python).
* **Directory Handling:** Appends the `images_dir` path to each image filename before function calls (Functionality likely implemented in Python).
* **Classifier Invocation:** Processes classifier outputs by converting them to lowercase and removing whitespace. Classifies labels as dogs, marking correct classifications with `1` and incorrect ones with `0` (Functionality likely implemented in Python).
* **Result Verification:** Ensures all matches and non-matches are displayed correctly and verifies model performance (Functionality likely implemented in Python).

## Results
- **Model Performance:** All three models (AlexNet, ResNet, and VGG) performed as expected.

## Additional Questions Answered

### 1. Did the three model architectures classify the breed of the dog in `Dog_01.jpg` as the same breed?
**Answer:** Yes, all three model architectures (AlexNet, ResNet, and VGG) correctly identified the breed of the dog in `Dog_01.jpg` as "Basenji."

### 2. Did each model architecture classify the breed of `Dog_01.jpg` as the same breed as that of `Dog_02.jpg`?
**Answer:** Yes, all three models (AlexNet, ResNet, and VGG) classified both `Dog_01.jpg` and `Dog_02.jpg` as "Basenji."

### 3. Did the models correctly classify `Animal_Name_01.jpg` and `Object_Name_01.jpg` as not being dogs?
**Answer:** Yes, all three models correctly classified `Animal_Name_01.jpg` (Fox_Squirrel_01.jpg) and `Object_Name_01.jpg` (Coffee_Mug_01.jpg) as non-dogs.

### 4. Based on the above answers, which model architecture performed the best?
**Answer:** Since all three models performed accurately, VGG is selected as the best due to its consistent performance in correctly classifying all images.

## Feedback: 
<img width="905" alt="Screenshot 2024-08-17 at 14 58 17" src="https://github.com/user-attachments/assets/dbee669c-f80a-493a-b171-c2dc50f6bfa0">
<img width="882" alt="Screenshot 2024-08-17 at 14 59 08" src="https://github.com/user-attachments/assets/90b9427f-16ec-4a8f-8d2d-dc4d9c829d02">
<img width="875" alt="Screenshot 2024-08-17 at 14 59 24" src="https://github.com/user-attachments/assets/f6bd3841-eb5f-486b-bee7-ddd03a305bd9">


