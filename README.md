# Hand Gesture Controlled Virtual Mouse

This project implements a virtual mouse that can be controlled using hand gestures, offering a touch-free way to interact with your computer. By leveraging computer vision and hand-tracking technology, this system can move the cursor, perform clicks, take screenshots, and more — all using simple hand movements in front of your webcam.

Features

* **Cursor Movement**: Move your index finger to move the mouse pointer on screen.
* **Left Click**: Specific finger gesture triggers a left mouse click.
* **Right Click**: Another gesture simulates a right click.
* **Double Click**: Use combined gestures to trigger a double click.
* **Screenshot Capture**: Pinch gesture allows you to take a screenshot and save it.
* **Gesture Detection**: Uses Mediapipe's real-time hand tracking for detecting gestures.

## Technologies Used

* Python
* OpenCV
* MediaPipe
* PyAutoGUI
* Pynput

## How It Works

* The webcam captures real-time video.
* MediaPipe detects hand landmarks.
* Based on specific angles between fingers and distances (calculated via a utility script), predefined gestures are recognized.
* Corresponding mouse operations are triggered using PyAutoGUI or Pynput.

## Requirements

Make sure you have the following Python libraries installed:

```
opencv-python
mediapipe
pyautogui
pynput
```

You can install them using pip:

```bash
pip install opencv-python mediapipe pyautogui pynput
```

## How to Run

1. Clone the repository.
2. Make sure your webcam is connected and working.
3. Run the script:

```bash
python main.py
```

4. Use your hand in front of the webcam to control the mouse.

## Notes

* Make sure there is sufficient lighting for better hand detection.
* The gestures should be performed clearly to avoid misinterpretation.
* You may need to calibrate gestures for different screen sizes or hand positions.

---

Let me know if you'd like a sample folder structure or to add a `util.py` explanation too.
