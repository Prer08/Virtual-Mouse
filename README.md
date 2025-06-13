# 🖐️ Hand Gesture Mouse Control using OpenCV

A mini-project that demonstrates how to control the mouse using hand gestures via a webcam using OpenCV and Python. This system captures real-time hand movements and performs actions like **moving the cursor**, **left-click**, **right-click**, **double-click**, and **screenshot** — all touch-free.

---

## 🧠 Overview

This project showcases how **computer vision** and **gesture recognition** can be combined to build an intuitive and futuristic alternative to physical input devices. It uses **MediaPipe Hands** for landmark detection and **PyAutoGUI** for system control.

---

## 🎯 Features

- 🖱️ Move cursor with your index finger
- 👆 Left-click using middle finger gesture
- 👉 Right-click using index finger gesture
- ✌️ Double-click using both fingers
- 📸 Take screenshot with a palm fold gesture
- 🪟 Real-time tracking and interaction

---

## 🛠 Tech Stack

- **Language**: Python 3.x
- **Libraries**:
  - `OpenCV` – for video capture and image processing
  - `MediaPipe` – for hand landmark detection
  - `PyAutoGUI` – for mouse and screen control
  - `NumPy` – for mathematical operations
  - `Pynput` – for precise mouse actions

---

## 📂 Project Structure
├── virtual_mouse.py # Main script
├── util.py # Utility functions (angles, distances)
├── README.md # Project documentation
├── requirements.txt # List of dependencies


---

## 🧪 Requirements

### ✅ Software:
- Python 3.6 or later
- OpenCV (`cv2`)
- MediaPipe
- PyAutoGUI
- Pynput
- NumPy

### ✅ Hardware:
- A laptop/PC with webcam
- Windows OS (tested)

---

## 🔧 Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/hand-gesture-mouse.git
cd hand-gesture-mouse

# Create a virtual environment (optional)
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate (Windows)

# Install dependencies
pip install -r requirements.txt

##How to Run
python virtual_mouse.py
Ensure your webcam is on.

Move your hand in front of the camera.

Use gestures to control your mouse

Gesture Logic (Sample)
Action	Gesture Description
Move Cursor	Index finger tip tracked continuously
Left Click	Angle threshold between joints of middle finger
Right Click	Angle threshold between joints of index finger
Double Click	Two-finger press gesture
Screenshot	Thumb and index close together + palm in
