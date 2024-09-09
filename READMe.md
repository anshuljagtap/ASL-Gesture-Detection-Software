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
| B | ![Gesture B](./path_to_your_image/Screenshot 2024-09-09 at 6.23.49 PM.png) |
| Thank You | ![Gesture Thank You](./path_to_your_image/Screenshot 2024-09-09 at 6.38.54 PM.png) |

## Model Training
The data was labeled and trained using a simple convolutional neural network (CNN) using TensorFlow/Keras. The training was performed using **Google Teachable Machine**, where gestures were classified based on their image inputs. Below is a screenshot of the training pipeline:

![Training pipeline](./path_to_your_image/Google_teachable.png)

## Results
The model has shown promising results, with accurate classifications of the following gestures:
- A
- B
- C
- D
- Thank You

Here’s an example of a successful prediction for the **Thank You** gesture:

![Thank You Prediction](./path_to_your_image/Screenshot 2024-09-09 at 6.38.54 PM.png)

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ASL-Detection.git














"/Users/anshuljagtap/Desktop/Personal Projects/ASL Detection/venv/bin/python" "/Users/anshuljagtap/Desktop/Personal Projects/ASL Detection/test.py"
"/Users/anshuljagtap/Desktop/Personal Projects/ASL Detection/venv/bin/python" "/Users/anshuljagtap/Desktop/Personal Projects/ASL Detection/dataCollection.py"