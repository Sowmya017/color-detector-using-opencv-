## Yellow Color Detection Using OpenCV
# Overview
This project uses OpenCV, NumPy, and PIL to detect yellow-colored objects in real time from your webcam.
It works by converting each video frame into the HSV color space, creating a mask for the yellow range, and drawing a bounding box around detected areas.

# Requirements
pip install opencv-python numpy pillow

# How It Works
- Capture video from the webcam using cv2.VideoCapture(0).
- Convert each frame from BGR → HSV.
- Use get_limits() to generate HSV range for yellow.
- Create a mask using cv2.inRange() to isolate yellow pixels.
- Convert the mask into a PIL image and get a bounding box (bbox).
- Draw a red rectangle on the original frame wherever yellow is detected.
- Display the result in real time.
