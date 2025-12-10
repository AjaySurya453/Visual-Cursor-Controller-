# Eye-Controlled Mouse 👁️🖱️

An AI-powered virtual mouse that allows users to control the cursor and perform clicks using only eye movements and blinks. This project leverages **OpenCV** and **MediaPipe** for real-time facial landmark detection and **PyAutoGUI** for mouse control.

## 🚀 Features
- **Hands-Free Navigation:** Control the mouse cursor by simply looking at different areas of the screen.
- **Blink to Click:** Perform a left mouse click by blinking.
- **Real-Time Tracking:** Uses MediaPipe's efficient Face Mesh for low-latency performance.
- **Cross-Platform:** Works on any system that supports Python and OpenCV.

## 🛠️ Tech Stack
- **Python**
- **OpenCV:** For video capture and image processing.
- **MediaPipe:** For high-fidelity face and iris tracking.
- **PyAutoGUI:** For programmatically controlling the mouse cursor and clicks.

## 📦 Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/AjaySurya453/Visual-Cursor-Controller-.git
   cd eye-controlled-mouse
2.Install Dependencies Ensure you have Python installed, then run:
    pip install -r requirements.txt
🎮 How to Run
Connect a webcam to your computer.

Run the script:

python main.py

A window named "Eye Controlled Mouse" will appear.

🕹️ Controls
Move Cursor: The system tracks the iris of your eye. Look up, down, left, or right to move the cursor on your screen.

Click: Blink your left eye to perform a mouse click.

Note: The code calculates the vertical distance between eyelids to detect the blink.

⚙️ How It Works
Face Mesh Detection: The webcam feed is processed using MediaPipe to detect 478 3D facial landmarks.

Iris Tracking: Specific landmarks corresponding to the eye are tracked to determine the gaze direction.

Coordinate Mapping: The coordinates of the eye within the video frame are mapped to the screen resolution to move the cursor.

Blink Detection: The vertical distance between the upper and lower eyelids is calculated. If this distance drops below a specific threshold, a "click" action is triggered.

📝 Notes
Lighting: Ensure you are in a well-lit environment for the best tracking accuracy.

Position: Sit directly in front of the camera for optimal calibration.

Exit: Press q (or close the window) to stop the program.

🤝 Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request if you have ideas for improvements (e.g., right-click functionality, scrolling, or smoothing algorithms).