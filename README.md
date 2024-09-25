# Tennis Ball Tracking Project

This project implements a real-time tennis ball tracking system using multiple object detection models: YOLO, Faster R-CNN, and SSD. The goal is to detect and track a tennis ball in video frames effectively while handling the challenges posed by its small size.

## Table of Contents

- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Models and Architectures](#models-and-architectures)
- [Challenges and Risks](#challenges-and-risks)
- [Conclusion](#conclusion)


## Technologies Used

- **OpenCV**: For video processing, frame extraction, and rendering the output video with detected bounding boxes.
- **YOLO (You Only Look Once)**: A fast and efficient object detection model used for real-time tracking.
- **Faster R-CNN**: A more accurate but computationally intensive model used for robust detection.
- **SSD (Single Shot MultiBox Detector)**: A model that balances speed and accuracy for detecting objects.

## Installation

To set up the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/houda2024/Tennis_Ball_tracking.git
   cd tennis-ball-tracking
   ```

2. Install the required dependencies:
   ```bash
   pip install opencv-python torch torchvision
   ```

3. Install YOLOv5:
   ```bash
   git clone https://github.com/ultralytics/yolov5.git
   cd yolov5
   pip install -r requirements.txt
   ```

4. Ensure that you have the trained YOLO model (e.g., `yolov5s.pt`) in the appropriate directory.

## Usage

1. Update the video path and output folder in the code as necessary.
2. Run :
   
   ```

3. The processed video with tracked objects will be saved in the specified output directory.

## Models and Architectures

1. **YOLO**:
   - Fast, real-time object detection model.
   - Suitable for detecting small objects but may have accuracy limitations.

2. **Faster R-CNN**:
   - Two-stage detector known for high accuracy.
   - More computationally intensive, which may affect real-time performance.

3. **SSD**:
   - Single-shot detector providing a good balance between speed and accuracy.
   - Effective for detecting objects of varying sizes.

## Challenges and Risks

- **Small Object Detection**: The small size of the tennis ball can lead to challenges in accurately detecting and tracking it.
- **Computational Intensity**: Faster R-CNN's complexity can slow down processing times, especially for long videos.
- **False Positives/Negatives**: Models may misclassify background objects or fail to detect the ball, impacting overall reliability.

## Conclusion

This project showcases the integration of multiple object detection models to track a tennis ball in video frames. Understanding the strengths and weaknesses of each model is essential for optimizing performance and achieving accurate results.


