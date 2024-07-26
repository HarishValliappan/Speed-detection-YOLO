# Speed Detection Project

## Introduction
This project demonstrates a vehicle speed detection system using a YOLO object detection model and OpenCV. The system captures video footage of vehicles passing through a frame and calculates their speeds based on the time taken to cross two predefined lines.

## Features
- **Real-time vehicle detection:** Utilizes the YOLO object detection model to detect vehicles in each frame.
- **Speed calculation:** Computes vehicle speed based on the time taken to cross two predefined lines.
- **Bounding boxes:** Draws bounding boxes around detected vehicles with ID and speed annotation.
- **Frame saving:** Saves processed frames for further analysis.
- **Video output:** Outputs a video file with annotated vehicle speeds.

## Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/speed-detection-project.git
   cd speed-detection-project
2. **Install required libraries:**
   '''bash
   pip install -r requirements.txt
3. **Download the YOLO model weights:**
   Download the yolov8s.pt model file from the official YOLO repository and place it in the project directory.

## Usage

### Prepare your input video:
Ensure you have a video file named `video/highway.mp4` in the project directory or update the code to reflect the path to your video file.

### Run the speed detection script:
```bash
python speed_detection.py

### View the output:
The processed video with annotated vehicle speeds will be saved as output video.mp4 in the project directory.

## Methodology
- **Object Detection:** The YOLO model is used to detect vehicles in each frame of the input video.
- **Tracking:** The center points of detected vehicles are tracked to determine when they cross predefined lines.
- **Speed Calculation:** The speed of each vehicle is calculated based on the time it takes to travel between the two lines.
- **Annotation:** The calculated speed and vehicle ID are annotated on the output video frames.

## Results
You can view a sample output video demonstrating the speed detection capabilities of the system here: [Output Video](path/to/your/output.mp4)

## Note
The speed detection accuracy improves with more powerful GPUs, as they enable faster and more precise frame processing.
