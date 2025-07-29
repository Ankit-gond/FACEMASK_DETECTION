# FACEMASK_DETECTION
# Mask Detection Web App using OpenCV and Flask

A real-time webcam-based application that detects whether a person is wearing a face mask or not, using Haar Cascade classifiers. The system analyzes eye and face detection to infer mask presence.

## 📌 Features

- Detects faces and eyes in real-time using OpenCV Haar cascades
- Infers if a person is wearing a mask based on face/eye visibility
- Live video stream via webcam rendered in a web browser using Flask
- Displays real-time feedback: "Person Wearing Mask" or "Person not Wearing Mask"

## 🛠️ Tech Stack

- Python
- Flask
- OpenCV
- HTML (for the front-end interface)

## 🚀 How it Works

1. The webcam feed is captured using OpenCV.
2. Haar cascades detect eyes and faces from the frame.
3. If eyes are detected **but face is not**, it's assumed the person is wearing a mask.
4. The app displays a corresponding message on the frame and streams it live via Flask.

## 📂 Project Structure

mask-detection-app/
├── app.py
├── templates/
│ └── index.html
├── haarcascade_frontalface_default.xml
├── haarcascade_eye.xml
└── README.md

```bash
git clone https://github.com/yourusername/mask-detection-webapp.git
cd mask-detection-webapp

## **Install Requirements**
pip install opencv-python flask

Make sure haarcascade_frontalface_default.xml and haarcascade_eye.xml are present in the root directory.
You can get them from the OpenCV GitHub:

  1.Face Cascade
  2.Eye Cascade
