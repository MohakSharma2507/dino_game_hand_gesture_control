Dino Game Hand Gesture Control
This project implements a hand gesture-controlled version of the popular Chrome Dino game using computer vision. The hand tracking is achieved through OpenCV, MediaPipe, and CVZone libraries, allowing users to control the Dino's movements (like jumping) with simple hand gestures.

Project Features:

Hand Tracking: Uses MediaPipe and CVZone to detect and track hand movements in real-time via webcam.
Gesture Recognition: Identifies hand gestures such as pinching or the distance between fingers to simulate keypresses for game control.
Seamless Game Control: Uses the pyautogui library to simulate keyboard presses (e.g., jumping in the Dino game).
Cross-Platform: Runs on multiple platforms, including macOS (tested on Mac M3) and Windows.
Technical Details:

OpenCV: Used for video capture and real-time image processing.
MediaPipe: Utilized for hand landmark detection.
CVZone: Provides an easier interface for handling hand tracking and gesture recognition.
PyAutoGUI: Simulates the up key press to control the Dino jump based on hand gestures.
How it Works:

The webcam captures the hand movements in real time.
The hand landmarks (points) are tracked and analyzed to determine the distance between certain points (e.g., index and thumb).
If the distance between the tracked points falls below a threshold, it triggers the jump action in the Dino game using the pyautogui.press('up') function.
Technologies Used:

Python
OpenCV
MediaPipe
CVZone
PyAutoGUI
Future Enhancements:

Add more gestures for crouching or increasing speed.
Improve gesture sensitivity and robustness in various lighting conditions.
Check out the GitHub repository for the code and installation instructions.
