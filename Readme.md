# Pose Detection with OpenCV and MediaPipe

This repository contains a Python script for detecting and tracking poses in videos using OpenCV and MediaPipe. It utilizes the `PoseModule` class from the `PoseModule.py` file.

## Requirements

To run the script, you need to have the following dependencies installed:

- Python 3.x
- OpenCV
- MediaPipe

You can install the required dependencies using pip:

```
pip install opencv-python
pip install mediapipe
```
# Usage
1. Clone the repository and navigate to the project directory:
```
git clone <repository-url>
cd <repository-directory>
```
2. Prepare the input video file:
Make sure you have a video file in a supported format (e.g., MP4) that you want to analyze. Update the video_path variable in the pose_detection.py script to specify the path to your video file:
```
cap = cv2.VideoCapture("path/to/your/video.mp4")
```
3. Run the pose detection script:
Execute the poseProject.py script to run the pose detection algorithm on the video:
```
python poseProject.py
```
4. View the results:
The script will display the processed video with pose landmarks and additional visualizations. The position of the right elbow will be highlighted with a red circle. The frame rate (FPS) will be shown in the top-left corner of the video.

# Customization
You can customize various parameters in the PoseDetector class of the PoseModule.py file:

* mode: Whether to detect the full body or just the upper body (default: False).
* complexity: The complexity of the pose landmark model (default: False).
* enableSeg: Whether to enable segmentation overlay (default: False).
* smooth: Whether to smooth the pose landmarks (default: True).
* detectionCon: Detection confidence threshold (default: 0.5).
* trackCon: Tracking confidence threshold (default: 0.5).
Feel free to modify these parameters to suit your needs.