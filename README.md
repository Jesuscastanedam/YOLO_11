# YOLO 11 Object Detection Explorer

## Description

This project uses YOLO 11, the latest object detection model from Ultralytics, to perform real-time recognition through webcam. The code is adapted from the work of **Albert Coronado Calzada**.

## Features

- Real-time object detection using YOLO 11
- Integrated webcam interface
- Bounding box visualization with confidence labels
- Support for 80+ object classes (COCO dataset)

## Environment Setup

### 1. Create virtual environment

```bash
# Create virtual environment
virtualenv venv 

# Activate virtual environment
# Linux/Mac:
source venv/bin/activate

# Windows:
venv\Scripts\activate
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

Main dependencies include:
- ultralytics
- opencv-python
- torch

### Controls

- **'q'**: Press to exit the application

## Functionality

The system:

1. Loads the pre-trained YOLO 11 model (`yolo11l.pt`)
2. Captures video in real-time from your webcam
3. Processes each frame to detect objects
4. Draws bounding boxes around detected objects
5. Displays object name and confidence level

## Experimental Results

During testing, the model demonstrated:

**Successful detections:**
- People
- Mobile devices (iPhone)
- Water bottles

**Observed limitations:**
- Confusion between small objects (e.g., Luigi figure detected as cake)

This illustrates both the potential and current limitations of computer vision systems, which depend on the model's training data.

## Project Structure

```
.
├── Explorer.ipynb          # Main notebook with step-by-step analysis
├── requirements.txt        # Project dependencies
└── README.md               # This file
```

## YOLO 11 Model

YOLO 11 represents the state of the art in object detection, offering:
- Higher precision than previous versions
- Optimized real-time processing
- Support for multiple computer vision tasks

## Credits

Code adapted from the work of **Albert Coronado Calzada**.

Based on YOLO 11 model from [Ultralytics](https://docs.ultralytics.com/models/yolo11/).

## Potential Applications

This type of technology has infinite applications:
- Intelligent security systems
- Retail and manufacturing applications
- Behavioral analysis
- Robotics and autonomous vehicles
- Medical and health applications

## License

This project is for educational and experimental purposes.