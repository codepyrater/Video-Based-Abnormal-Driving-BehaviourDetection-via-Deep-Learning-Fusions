# Video-Based Abnormal Driving Behavior Detection via Deep Learning Fusions

This project implements a system to detect abnormal driving behaviors from video footage using a Convolutional Neural Network (CNN). The system identifies behaviors such as safe driving, talking on the phone, drinking, reaching behind, and more.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [How It Works](#how-it-works)
- [Future Enhancements](#future-enhancements)
- [License](#license)

## Overview
The system processes video footage frame by frame to detect and classify different driving behaviors. It uses a pre-trained CNN model to analyze each frame and determine if the driver is engaging in any abnormal behavior. The detected behavior is then displayed on the video feed in real-time.

## Features
- Generate and load the Abnormal Driving Behavior Detection (AWGRD) model
- Upload and process video footage
- Real-time detection and classification of driving behaviors
- Display detected behaviors on the video feed

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/abnormal-driving-detection.git
    cd abnormal-driving-detection
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Run the main application:
    ```bash
    python main.py
    ```
2. Generate and load the AWGRD model by clicking the "Generate & Load AWGRD Model" button.
3. Upload a video by clicking the "Upload Video" button.
4. Start monitoring the video by clicking the "Start Behaviour Monitoring" button.
5. To exit the application, click the "Exit" button.

## Project Structure
abnormal-driving-detection/
│
├── dataset/ # Folder containing training and validation datasets
├── main.py # Main application script
├── README.md # Project README file
├── requirements.txt # List of dependencies
└── AWGRD_model.h5 # Pre-trained model weights (if available)

markdown
Copy code

## Dependencies
- Python 3.x
- NumPy
- OpenCV
- Keras
- TensorFlow
- Tkinter
- imutils
- dlib

## How It Works
1. **Model Generation and Loading:** The system generates and loads the AWGRD model, which is a CNN trained on a dataset of driving behaviors. If the model weights file (`AWGRD_model.h5`) is available, it will load the pre-trained weights.
2. **Video Upload:** The user uploads a video file containing driving footage.
3. **Behavior Monitoring:** The system processes the video frame by frame. For each frame, the system:
   - Extracts the frame and resizes it to the required input size for the model.
   - Predicts the driving behavior using the AWGRD model.
   - Displays the detected behavior on the video feed.
4. **Output:** The detected behavior is displayed on each frame of the video in real-time.

## Future Enhancements
- Improve the accuracy of the model by training on a larger and more diverse dataset.
- Implement support for real-time video feed from a camera.
- Add more classes of driving behaviors for detection.
- Enhance the user interface for better usability.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to contribute to this project by submitting issues or pull requests.