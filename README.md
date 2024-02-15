# Wireless-Sound-Control

This repository contains a python project that utilizes computer vision techniques along with audio processing to create a hand gesture-controlled volume adjustment system. It enables user to control the audio volume of their system using hand gestures captured via a webcam. The system detects specific hand gestures of pinching fingers together and adjusts the volume accordingly. 

## Getting started
### Dependencies
- Python
- OpenCV
- Mediapipe
- Numpy
- pycaw
- ctypes
- comtypes

### Installation and Usage
1. Clone this repository to your local machine.
2. Install the required dependencies. You can install them using pip.
3. Run the 'WirelessSoundControl.py' script.
4. Point your webcam towwards your hand, and perform the gesture to control the volume (eg. pinching fingers together)
5. The system will adjust the audio volume based on the detected. hand gesture.

## Features
- **Hand Gesture Detection:** Utilizes the Mediapipe library for hand tracking and landmark detection.
- **Real-Time Volume Adjustment:** Adjusts the system's audio volume in real-time based on detected hand gestures.
- **Visual Feedback:** Provides visual feedback on the webcam feed, indicating the detected hand positions and the current volume level.

## How it works
The system utilizes computer vision techniques to detect and track hand gestures in real-time. It captures video frames from the webcam, processes them to detect hand landmarks using the Mediapipe library, and calculates the distance between specific landmarks to recognize gestures. It uses the distance between the tip of your index finger to the tip of your thumb as a measure of volume.

Once a gesture is recognized, the system maps the gesture length to the volume range and adjusts the system's audio volume accordingly using the pycaw library.

## Acknowledment
Project under Coincent program of _Data Science with Python_.
