# Color-Based Object Detection (Project #02)

The second project in my **AI/ML Learning Path**. This project moves from detecting general motion to isolating and tracking objects based on specific color features.

## 📌 Overview
This script identifies and tracks objects of a specific color in a real-time video stream. By utilizing the HSV (Hue, Saturation, Value) color space, the system can reliably filter out background data and focus on a target object.

## 🛠️ Tech Stack
* **Language:** Python
- **Library:** OpenCV
- **Concepts:** HSV Color Space, Color Masking, Morphological Operations (Erosion/Dilation), Contour Tracking.

## ⚙️ How It Works
1. **Color Space Conversion:** Converts frames from BGR to HSV for more robust color filtering.
2. **Thresholding:** Creates a binary mask where the target color appears white and everything else is black.
3. **Morphological Filtering:** Uses dilation and erosion to remove small "noise" dots from the mask.
4. **Object Localization:** Finds the largest contour in the mask and draws a bounding box or center point around it.

## 🚀 Quick Start
1. Install OpenCV: `pip install opencv-python`
2. Run the script: `python main.py`
3. Adjust the HSV values in the code to target your specific object (default is set to a specific color range).

---
*Progress: Moving from basic motion to specific feature extraction. Next: Multi-object tracking!*
