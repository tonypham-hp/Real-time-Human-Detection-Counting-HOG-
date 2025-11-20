# Real-time Human Detection & Counting using HOG (OpenCV, Python)

## Project Overview  
This project implements a real-time people detection and counting system using Python & OpenCV’s HOG (Histogram of Oriented Gradients) + SVM. It supports input via webcam, video file, or image file.  

## Features  
- Detect humans in real-time from webcam, video, or image.  
- Draw bounding boxes and labels for each person detected.  
- Display total count of persons present.  
- Optionally save output to image or video file.

### Prerequisites  
- Python 3.x  
- Libraries:  
  ```bash
  pip install opencv-python  
  pip install imutils  
  pip install numpy

## Folder Structure
Real-time-Human-Detection-Counting-HOG-/

├── image/                     ← sample images    
├── video/                     ← sample video files     
├── human_counting.py          ← main Python script  
├── README.md                  ← this file  
└── …                        

## Running the Project
From terminal (at repository root):
- Webcam mode:
    ``` bash
  python human_counting.py --camera true  
- Video mode:
  ```
  python human_counting.py --video path/to/video.mp4  
- Image mode:
    ``` bash
    python human_counting.py --image path/to/image.jpg  
- Save output (video or image):
    ```bash
    python human_counting.py --video path/to/video.mp4 --output output_filename.avi  
    python human_counting.py --image path/to/image.jpg --output output_image.jpg


## Notes & Limitations

- HOG + SVM works well for upright, clearly visible standing persons. May miss people in complex scenes (e.g., occlusions, groups, varied poses).

- For more accurate results (especially crowded or complex scenes), consider modern detectors (e.g., YOLO, SSD).

- Ensure your camera/video feed has sufficient resolution and lighting for better detection.
