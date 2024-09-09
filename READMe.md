# ASL Hand Gesture Detection 

This project is focused on detecting American Sign Language (ASL) gestures using OpenCV, cvzone, and TensorFlow/Keras for hand gesture classification. The goal is to build a real-time system that can recognize and classify different ASL hand signs.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Collection](#data-collection)
3. [Model Training](#model-training)
4. [Results](#results)
5. [How to Run](#how-to-run)
6. [Future Work](#future-work) 

## Project Overview
The project utilizes computer vision techniques and a pre-trained model to classify hand gestures. The application tracks a user's hand, extracts the region of interest (ROI), and then uses a deep learning model for classification. The current model is capable of recognizing gestures such as **A**, **B**, **C**, **D**, and **Thank You**.(The model can be trained to add endless hand gestures for sign language )

## Technologies used: 
- Python - Programming language used for building the project.
- OpenCV - For hand tracking and image processing.
- cvzone - For easier integration with OpenCV and hand detection functionality.
- TensorFlow/Keras - Deep learning framework used to train and classify the hand gestures.
- Teachable Machine - Google's web-based tool used for training the gesture classification model.
- NumPy - For array manipulations and mathematical operations.
- Math - For calculations related to aspect ratios and image resizing.
- Time - Used for handling delays and naming image files during data collection.
- MediaPipe - (Indirectly through cvzone) for hand landmark detection.

### ASL Detection in action

## Data Collection
Data for the model was collected using the webcam. The hand was detected, and images of different ASL signs were saved after cropping and resizing.

Here is the data collection process for "Thank you":
<img width="1440" alt="Thank you detection" src="https://github.com/user-attachments/assets/2f939f22-cea6-4141-990f-377ee7ab804f">


Project Images/Thank you data training.png 


| Gesture | Example |
|---------|---------|
| A | <img width="1440" alt="A detection" src="https://github.com/user-attachments/assets/4e26d400-18e2-4f99-bf08-baf7e8397d66"> |
| B | <img width="1440" alt="B detection" src="https://github.com/user-attachments/assets/7edfd8ad-1bd3-40e6-8e12-fa4716b42b00"> |
| Thank You | <img width="1440" alt="Thank you data training" src="https://github.com/user-attachments/assets/6128c6bf-2461-4ac2-a31d-444b4c54d1fa">|

## Model Training
The data was labeled and trained using a simple convolutional neural network (CNN) using TensorFlow/Keras. The training was performed using **Google Teachable Machine**, where gestures were classified based on their image inputs. Below is a screenshot of the training pipeline:

<img width="1431" alt="Google teachable" src="https://github.com/user-attachments/assets/83dd86dc-87f8-4784-acad-1cb4817fad3e">

## Results
The model has shown promising results, with accurate classifications of the following gestures:
- A
- B
- C
- D
- Thank You





## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ASL-Gesture-Detection-Software.git




"/Users/<username>/Desktop/Personal Projects/ASL Detection/venv/bin/python" "/Users/<username>/Desktop/Personal Projects/ASL Detection/test.py"
"/Users/<username>/Desktop/Personal Projects/ASL Detection/venv/bin/python" "/Users/<username>/Desktop/Personal Projects/ASL Detection/dataCollection.py"
