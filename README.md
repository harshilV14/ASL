
# 🤟 ASL to Text

The **ASL to Text Converter** is a project aimed at translating American Sign Language (ASL) hand gestures into written text. This tool leverages machine learning and computer vision techniques to interpret sign language and provide accurate translations, making communication more accessible for deaf and hard-of-hearing individuals.

## 🚀 Features

- **Real-time Gesture Recognition**: Translates ASL signs into text instantly.
- **High Accuracy**: Built on a robust machine learning model trained on a diverse dataset.
- **Intuitive Interface**: User-friendly design for seamless interaction.
- **Customizable Vocabulary**: Users can add or modify signs for personal use.

## 🛠 Built With

We have mainly used Python and some of its libraries and tools to build this project. Some of these are:

- **🟡 cvzone**: Used to access the camera to capture hand gestures, including the built-in `HandDetector` library for hand detection.
  
- **🔢 Numpy**: Used for model predictions, specifically for predicting different hand signs and the letters used.

- **🖐 Mediapipe**: A cross-platform framework developed by Google for processing video and multimedia. It provides advanced capabilities for hand tracking and gesture recognition, making it ideal for real-time ASL recognition.

- **🔍 OpenCV**: An open-source computer vision and machine learning library that provides tools for image and video processing, essential for capturing and manipulating frames from a webcam.

- **🧠 TensorFlow**: An open-source machine learning framework developed by Google, widely used for building and training machine learning models. In this project, TensorFlow runs the neural network model that recognizes ASL gestures.

- **🤖 Teachable Machine**: A user-friendly web tool that allows anyone to create machine learning models without coding, designed for tasks like image classification and pose detection.

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ChirayuDodiya/ASL-to-Text

    Install required packages: 
    pip install -r requirements.txt

## 🏗 Process Overview

The process of developing the ASL to Text Converter involves three main steps: data collection, model training, and testing. Here's how each step works:

### 1. Data Collection

- **File**: `collect.py`
- **Description**: This script is used to collect data for training the model. 
- **How It Works**:
  1. Run the `collect.py` script.
  2. The script opens a user interface where you can click on letters to indicate the corresponding ASL sign. The Data is stored in \Data folder.
  3. Each click records the hand gesture as a data sample, which is saved for training.

### 2. Model Training

- **Tool**: Teachable Machine by Google
- **Description**: The collected data is uploaded to Teachable Machine, where it is used to train the model.
- **How It Works**:
  1. Once you have collected sufficient data, export it from `collect.py`.
  2. Upload the dataset to Teachable Machine.
  3. Train the model using the uploaded data to recognize the ASL signs.
  4. After training, export the model as a Keras model file (usually in `.h5` format).

### 3. Testing

- **File**: `test.py`
- **Description**: This script is used to test the trained model.
- **How It Works**:
  1. Run the `test.py` script.
  2. The script loads the trained Keras model.
  3. It accesses the camera to capture live hand gestures.
  4. The model predicts the corresponding ASL sign in real-time, displaying the recognized letter on the screen.





## 🤝 Contributors

- [@Chirayu Dodiya](https://github.com/ChirayuDodiya)
- [@Mayank](https://github.com/likemacc)
- [@Nandini Gadhvi](https://github.com/NadiniGadhvi)
- [@Abhishek Guna](https://github.com/HINOKAM-ii)
- [@Harshil Vasava](https://github.com/harshilV14)


## Demo

Insert gif or link to demo

