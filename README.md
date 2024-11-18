# Soccer Player and Ball Tracking using Faster R-CNN and Deep SORT

This project implements a comprehensive system for detecting and tracking soccer players and the ball in video footage using **Faster R-CNN** for object detection and **Deep SORT** for multi-object tracking. It is designed to provide an efficient way to analyze soccer matches, offering real-time tracking and visual feedback.

## Project Overview

In this project, we leverage **Faster R-CNN** to detect objects (soccer players and the ball) within each frame of a video, and use **Deep SORT** to track those objects across multiple frames. The system is capable of handling real-time video processing and outputs annotated video with visual markers on tracked players and the ball.

### Key Objectives:
- **Object Detection**: Detect soccer players and the ball using Faster R-CNN.
- **Object Tracking**: Track detected objects (players and the ball) in real-time across frames using Deep SORT.
- **Visualization**: Annotate the video with bounding boxes and IDs for both players and the ball, making it easier to analyze player movements and ball trajectories.

## Features

- **Real-time detection and tracking** of soccer players and the ball.
- **Visualization**: Bounding boxes and unique IDs are assigned to each player and ball for easy tracking.
- **Multiple video format support** for input and output files.
- **Pre-trained models** for Faster R-CNN and Deep SORT.
- **Customizable**: Can be adapted to various video formats and different sports.

## Technologies Used

- **Python**: The primary programming language for the project.
- **Faster R-CNN**: A deep learning object detection algorithm used for detecting players and the ball in each frame.
- **Deep SORT**: A multi-object tracking algorithm used to track the detected players and the ball across video frames.
- **OpenCV**: A computer vision library used to process and display the video frames.
- **PyTorch**: A deep learning framework used to implement Faster R-CNN.
- **NumPy**: For handling numerical operations and matrix manipulations.
- **Matplotlib**: Used for plotting, if needed for data visualization (e.g., trajectory plots).

## Installation

Follow the steps below to set up the project on your local machine:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/SolomonMartin/Soccer-Player-and-Ball-Tracking-using-Faster-R-CNN-and-Deep-SORT.git

2. **Naavigate to the project directory**:
    ```bash
    cd Soccer-Player-and-Ball-Tracking-using-Faster-R-CNN-and-Deep-SORT

3. **Install the required dependencies**:
    ```bash
    pip install opencv-python-headless
    pip install torch torchvision torchaudio
    pip install numpy
    pip install matplotlib
    pip install deep-sort-realtime

4. **Specify the appropriate file location to save the files**

5. **Run the cells in order**


## How It Works
1. **Faster R-CNN** detects soccer players and the ball in each frame by generating bounding boxes around the objects and classifying them.
2. **Deep SORT** assigns a unique ID to each detected object and tracks them across subsequent frames, ensuring consistent tracking of players and the ball.
3. **OpenCV** is used to visualize the results by overlaying the bounding boxes and IDs on the video frames and saving the annotated output.