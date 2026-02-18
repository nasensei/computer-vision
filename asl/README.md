# 🖐️ Real-Time Hand Sign Language Recognition

A real-time computer vision system for detecting and classifying hand sign language letters using YOLO and Python.

This project was developed as a collaborative end-to-end machine learning system, covering data collection, model training, evaluation, and live inference.

---

## 🚀 Overview

This system uses a YOLO-based object detection model to:

- Detect hand signs from live webcam input
- Classify sign language letters (A–Z)
- Display real-time bounding boxes and predictions
- Operate with low latency for smooth live interaction

The project demonstrates:

- End-to-end ML pipeline design  
- Real-time inference system development  
- Model optimisation under real-world conditions  

---

## 🛠 Tech Stack

**Language**
- Python

**Libraries & Frameworks**
- YOLO (Ultralytics)
- OpenCV
- PyTorch
- NumPy

**Tools**
- Git & GitHub
- Jupyter Notebook (`ASL_classification.ipynb`)

---

## 📂 Project Structure
# 🖐️ Real-Time Hand Sign Language Recognition

A real-time computer vision system for detecting and classifying hand sign language letters using YOLO and Python.

This project was developed as a collaborative end-to-end machine learning system, covering data collection, model training, evaluation, and live inference.

---

## 🚀 Overview

This system uses a YOLO-based object detection model to:

- Detect hand signs from live webcam input
- Classify sign language letters (A–Z)
- Display real-time bounding boxes and predictions
- Operate with low latency for smooth live interaction

The project demonstrates:

- End-to-end ML pipeline design  
- Real-time inference system development  
- Model optimisation under real-world conditions  

---

## 🛠 Tech Stack

**Language**
- Python

**Libraries & Frameworks**
- YOLO (Ultralytics)
- OpenCV
- PyTorch
- NumPy

**Tools**
- Git & GitHub
- Jupyter Notebook (`ASL_classification.ipynb`)

---

## 📂 Project Structure
│
├── data/
│   ├── raw_images/
│   ├── labelled_images/
│   └── dataset.yaml
│
├── training/
│   ├── train.py
│   ├── results/
│
├── inference/
│   ├── detect_live.py
│
├── models/
│   ├── best.pt
│
└── ASL_classification.ipynb

---

## 📸 Data Collection & Labelling

1. Collected hand sign images using webcam.
2. Split dataset into training and validation sets.
3. Labelled images in YOLO format:class_id x_center y_center width height
4. Configured dataset using `dataset.yaml`.

---

## 🏋️ Model Training

Training was performed using YOLO with configurable hyperparameters.

Example:

```bash
yolo task=detect mode=train model=yolov8n.pt data=dataset.yaml epochs=50 imgsz=640
