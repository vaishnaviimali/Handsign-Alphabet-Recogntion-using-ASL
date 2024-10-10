# Handsign Alphabet Recognition-usingASL
This project focuses on real-time recognition of sign language alphabets, offering a seamless solution for bridging communication gaps between individuals who use sign language and those who do not. The system captures hand gestures via a webcam and classifies them into corresponding alphabets from the American Sign Language (ASL) alphabet.

Problem Statement:

Sign language is the primary method of communication for many people with hearing impairments. However, a significant communication barrier exists when interacting with people who are unfamiliar with sign language. This project aims to reduce this barrier by creating a system that can recognize and interpret sign language alphabets in real time, making it easier for non-signers to understand basic gestures without the need for a human translator.

Approach:

The system uses computer vision techniques to detect hand gestures, which are then classified into corresponding alphabetic characters. Key stages of the project include:

Hand Detection: Using MediaPipe and OpenCV, the system identifies and tracks the hand in a live video stream from the user's webcam. It then crops and processes the hand image for classification.
Real-Time Classification: A Convolutional Neural Network (CNN) is trained to recognize individual alphabetic signs. This model is trained using a custom dataset, which includes over 500-1000 images per letter to ensure high accuracy.
Dataset: A custom dataset of hand signs was collected, consisting of more than 500 images per letter. The data was carefully pre-processed to maintain uniformity and accuracy in training the model.
Preprocessing and Resizing: The cropped hand gesture is resized to maintain the aspect ratio, ensuring consistent input dimensions for the model. This is critical for the performance of the deep learning model.
Classification: TensorFlow and Google Teachable Machine are used to build and train the deep learning model. The system leverages a CNN to classify the input images, providing predictions in real time.
Technologies Used:
TensorFlow: For building and training the Convolutional Neural Network (CNN) used to classify the hand gestures into alphabets.
MediaPipe: For efficient and fast hand tracking, detection, and landmark identification.
Google Teachable Machine: To simplify the training and testing of the model, providing an intuitive interface for building machine learning models.
OpenCV: For video capture, hand gesture cropping, and real-time processing of hand images.
Python: For the overall integration of various modules and building the project pipeline.
Computer Vision: For hand tracking, preprocessing, and gesture recognition.
CNN (Convolutional Neural Network): For accurate and efficient classification of sign language alphabets.
Future Advancements:

As part of future improvements, the project aims to implement a predictive model that can anticipate the next alphabet based on the current recognized hand gesture. This would further enhance communication by reducing the need for redundant gestures and improving prediction speed. Additionally, expanding the model to recognize full words or sentences by incorporating sign language grammar is another long-term goal.

Key Features:

Real-time Detection: The system processes live video feeds to detect and classify hand gestures instantaneously.
Custom Dataset: Over 500-1000 images per alphabet are used to ensure robustness and accuracy of the model.
Accurate Classification: With the help of a CNN, the model achieves efficient and accurate classification results.
Seamless Interaction: A user-friendly interface and real-time feedback make the system practical for daily use.
How to Use:
Clone the repository and install the required dependencies.
Run the provided Python script to launch the system.
Use a webcam to display hand gestures, and the system will detect and classify the corresponding alphabet in real time.
