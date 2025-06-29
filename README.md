# AR Process Visualization & Image Filtering System

This project combines two key computer vision tasks:
1. Implementation and benchmarking of custom image filters.
2. Augmented reality image projection using ArUco markers.

---

## 📌 Task Overview

### 🧪 Task 1: Image Filter Implementation & Benchmarking

#### 🎯 Goal
Implement and compare custom and OpenCV versions of:
- Average filters (3x3, 5x5)
- Gaussian filters (3x3, 5x5)
- Sobel filter

#### ⚙️ Constraints
- No direct use of `cv.filter2D()` or `cv.GaussianBlur()`
- Only grayscale images
- Allowed: `cv.getGaussianKernel()` for kernel generation

#### 📊 Evaluation
- Compare output images with OpenCV equivalents
- Calculate and visualize difference images
- Measure and compare runtime using `cv.getTickCount()` or Python `time`

---

### 🕶️ Task 2: AR Marker-Based Image Augmentation

#### 🎯 Goal
Project an image onto a physical space detected via ArUco markers using homography and perspective warping.

#### 🔍 Functionality
- Detect ArUco markers via OpenCV (`cv2.aruco`)
- Compute homography between source and marker coordinates
- Warp and overlay a static image on the detected marker plane
- Expand marker area to exaggerate projection area

#### 🛠️ Used Libraries
- OpenCV (cv2)
- NumPy

#### 🖼️ Image Flow
**Left → Right**:
1. Input Frame  
2. Marker Detection  
3. Projected Image Augmentation  

---

## 🛠️ Tech Stack

- Python
- OpenCV (cv2, aruco)
- NumPy

---

## 📁 Project Structure

