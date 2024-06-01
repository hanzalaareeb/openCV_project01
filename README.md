# Augmented Reality with OpenCV

  This project demonstrates an agumented reality (AR) application using OpenCV. This application aptures real-time video from the webcam, detects a target image within the webcam feeed, and overlays a video onto the detected target image.

## Features
- Real-time video capture from the webcam.
- Detection of a target image within the webcam feed.
- overlay of a specified video onto the detected target image.

## Dependencies

  1) OpenCV
  2) NumPy
you can install dependencies using the following command:
     ```bash
     pip install opencv-python-headless numpy

## Code Explanation
- Intialization: The webcam and video files are loaded. ORB (Oriented FAST and Rotated BRIEF) is used to detect keypoints and descriptors in the target image
- Webcam Loop: Captures each frame from the webcam. If the target image is detected, the video is overlaid onto the target area.
- Feature Matching: Uses ORB to find keypoints in the current webcam frame and matches them to keypoints in the target image using BFMatcher.
- Homography and Warping: Computes the homography matrix to warp the video frame onto the target area in the webcam feed.
- Display: Shows the audmented reality feed along with feature matches for debugging purposes.
