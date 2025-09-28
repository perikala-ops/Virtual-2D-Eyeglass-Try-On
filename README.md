
***

# Virtual 2D Eyeglass Try-On

## Project Overview  
This project is a Python-based computer vision application that enables virtual try-on of eyeglasses on a static or real-time face image. Using Mediapipe for facial landmark detection and OpenCV for image transformation and overlay, the project aligns and scales eyeglasses based on eye landmarks to simulate realistic glasses fitting.

## Features  
- Precise detection of eye landmarks using Mediapipe Face Mesh  
- Calculations of eye distance, rotation angle, and mid-eye center for accurate glasses placement  
- Resizing, rotating, and transforming eyeglass images to match face orientation  
- Transparent overlay of eyeglasses with smooth edges using alpha channel handling  
- Visualization of results in static images and real-time video feed  

## How It Works  
The solution is implemented as a 4-step pipeline:  
1. **Eye Landmark Detection**  
   - Detect facial landmarks focusing on eye positions from an input face image.  
2. **Glasses Transformation**  
   - Compute required width, angle, and position transformations for the glasses image based on landmarks.  
3. **Overlay Process**  
   - Apply transparent overlay of transformed eyeglasses on the input face image.  
4. **Final Integration**  
   - Combine all steps to detect eyes, transform glasses, and overlay them either on static images or in real-time video.

## Getting Started  

### Prerequisites  
- Python 3.x  
- OpenCV  
- Mediapipe  
- Numpy  
- Matplotlib  

### Installation  
```bash
pip install opencv-python mediapipe numpy matplotlib
```

### Usage  
- Place your face image (`face.jpg`) and eyeglass PNG with transparency (`eyeglass.png`) in the working directory.  
- Run the Jupyter Notebook or Python script to execute the steps and visualize the eyeglass try-on.

## Code Structure  
- `Step1_Detect_Eye_Landmarks.ipynb` - Detects eye landmarks from face images.  
- `Step2_Transform_Glasses.py` - Resizes and rotates glasses based on eye landmarks.  
- `Step3_Overlay_Glasses.py` - Handles alpha blending to overlay glasses on faces.  
- `Step4_Integration.ipynb` - Connects all steps and displays final virtual try-on results.

## Technologies Used  
- Python  
- OpenCV  
- Mediapipe  
- Numpy  
- Matplotlib  

## Future Enhancements  
- Support for real-time video webcam input  
- 3D eyeglass try-on with depth estimation  
- Improved occlusion handling and multi-face detection  
- Integration with cloud-based deployment  

***
