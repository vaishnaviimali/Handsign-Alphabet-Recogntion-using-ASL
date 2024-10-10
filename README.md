# Sign Language Alphabet Recognition

## Overview

The **Sign Language Alphabet Recognition** project is aimed at providing real-time recognition of hand gestures representing the alphabets in American Sign Language (ASL). By leveraging deep learning and computer vision, this system can classify hand gestures into corresponding alphabetic characters with high accuracy. This solution helps bridge the communication gap between sign language users and non-sign language users.

### Problem Statement
Sign language is a critical method of communication for individuals with hearing impairments, but it can be challenging for non-signers to understand. This project aims to address this issue by creating a real-time system that recognizes hand gestures and translates them into alphabetic characters, enabling better interaction between sign language users and non-users.

### Key Features
- **Real-time Detection**: Detects and classifies hand gestures in real time from a live video stream.
- **High Accuracy**: The model is trained on a custom dataset containing over 500-1000 images per alphabet.
- **User-friendly Interface**: The system provides immediate feedback, displaying the recognized alphabet as the gesture is made.

## Technologies Used
- **TensorFlow**: For building and training the Convolutional Neural Network (CNN) that classifies hand gestures into alphabets.
- **MediaPipe**: For hand tracking and landmark identification, facilitating gesture detection.
- **Google Teachable Machine**: To simplify training and deploying machine learning models.
- **OpenCV**: For real-time video capture, hand detection, and image preprocessing.
- **Python**: For implementing the overall project pipeline.
- **Computer Vision**: For detecting and preprocessing hand gestures.

## Future Advancements
- **Next Alphabet Prediction**: We plan to implement a feature that predicts the next alphabet based on the recognized hand gesture.
- **Word & Sentence Recognition**: Expanding the model to recognize full words or sentences using sign language grammar.

## Dataset
The dataset for this project can be created manually using the provided data collection script. It consists of **500-1000 images per alphabet**, representing different hand gestures for each letter of the ASL alphabet.

### Dataset Collection
1. Use the **data collection script** to capture hand gesture images.
2. The images are saved in separate folders for each alphabet.

### Dataset Training
The dataset is trained on **Google Teachable Machine**, a user-friendly platform for creating machine learning models.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/vaishnaviimali/handsign-recognition-usingASL.git
    cd handsign-recognition-usingASL
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the **data collection script** to capture hand gesture images:
    ```bash
    python DataCollection.py
    ```

4. Train the dataset on **Google Teachable Machine**. Once trained, export the model.

5. Run the **testing script** to classify hand gestures in real time:
    ```bash
    python test.py
    ```
    
## Requirements

- Python
- TensorFlow
- OpenCV
- MediaPipe
- cvzone

Install all dependencies with:
```bash
pip install tensorflow opencv-python mediapipe cvzone numpy
```
## Folder Structure
```bash
├── Data/
│   ├── A/     # Folder for images of alphabet A
│   ├── B/     # Folder for images of alphabet B
│   └── ...    # Folders for other alphabets
├── DataCollection.py  # Script for collecting dataset images
├── test.py       # Script for testing the model in real-time
├── README.md           # This README file
└── requirements.txt    # List of required dependencies
```

## Usage
1. Data Collection
- Ensure your webcam is connected.
- Run the data_collection.py script to capture images of each alphabet gesture:
```bash
python data_collection.py
```
- Press 's' to save an image during capture. Images will be saved in folders corresponding to each alphabet.

2. Model Training
- Visit Google Teachable Machine.
- Upload your captured dataset for training.
- Train the model and export it.

3. Testing
- After training, create separate folder to save model and its labels after that use the test.py script to test the model with real-time hand gestures:
```bash
python test_model.py
```

Thank you for checking out this project! If you find it helpful, please consider giving it a ⭐️ on GitHub.




