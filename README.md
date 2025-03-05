# AI-facial-Recognition-System
Facial Recognition Project

Overview

This project implements a facial recognition system using OpenCV and the face_recognition library. It encodes facial images, captures live images via webcam, and matches them with stored encodings to mark attendance.

Dependencies

Ensure you have the following libraries installed:

Python 3.x

OpenCV

NumPy

Face Recognition

CSV (for attendance tracking)

Google Colab (if running in a cloud environment)

Dataset

The images used for facial recognition are stored in the directory /content/drive/MyDrive/new images. The system extracts and encodes faces from these images.

Steps in the Project

1. Preprocessing

Reads images from the specified directory.

Extracts the names of individuals from filenames.

Encodes facial features using face_recognition.face_encodings.

2. Attendance System

Matches detected faces with encoded images.

If a match is found, the individual's attendance is recorded in /content/drive/MyDrive/attendance.csv.

3. Capturing Live Images

Uses a webcam to capture real-time images.

Converts frames to RGB and detects faces.

Encodes and compares with stored face encodings.

Marks attendance if a match is found.

How to Run

Install dependencies using pip install face_recognition opencv-python numpy.

Ensure that the image dataset is placed in /content/drive/MyDrive/new images.

Run the script to encode and compare faces.

Attendance will be logged in attendance.csv.

Saving Attendance Data

The update_attendance function checks if a name already exists in attendance.csv.

If the name is new, it adds a new entry with the timestamp.

Notes

The threshold for face matching is set at 0.6.

Webcam access is required for real-time face recognition.

The script runs in a loop, continuously processing frames until the user exits.

Contact

For improvements or questions, feel free to reach out!

