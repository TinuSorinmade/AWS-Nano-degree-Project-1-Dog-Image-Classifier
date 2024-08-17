# Project Overview

This project is a component of the AWS AI & ML scholarship program offered through Udacity. The goal is to develop a command-line application in Python that uses a pre-trained image classifier, trained on the ImageNet dataset, to determine if an image depicts a dog and, if so, identify the breed of the dog.

## Project Requirements

The project meets the following requirements:

- **Timing Functions:** Calls time functions to measure the duration of the main code execution, both before and after the core logic.
- **Command Line Arguments:**
  - `--dir` (default: `pet_images/`): Directory containing the pet images.
  - `--arch` (default: `vgg`): Specifies the CNN architecture to use (e.g., VGG, ResNet, AlexNet).
  - `--dogfile` (default: `dognames.txt`): File containing the list of dog breeds.
- **File Handling:** Ensures that files starting with a dot (e.g., `.DS_Store`) are ignored using conditional statements.
- **Label Formatting:** Ensures dictionary keys and labels are in the correct format and retrieves 40 key-value pairs (e.g., `{'Poodle_07956.jpg': ['poodle'], 'fox_squirrel_01.jpg': ['fox squirrel'] ... }`).
- **Function Arguments:** Passes `in_arg.dir` as an argument to the `check_images.py` script while calling the `get_pet_labels` function.
- **Path Handling:** Appends `images_dir` to each value before making function calls.
- **Classification Output:** Converts classifier outputs to lowercase and removes any whitespace. Classifies labels as dogs with `1` for correct labels and `0` for incorrect classifications.
- **Output Verification:** Checks if all matches and non-matches are displayed correctly and verifies that all models perform as expected.

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


