# 🚗 YOLOv8 Object Detection on Self-Driving Car Data

This project implements real-time object detection using **YOLOv8** on datasets commonly used in **autonomous driving**. The model is trained to detect vehicles, pedestrians, traffic signs, and other road elements.

## 🔍 Overview

- **Model**: YOLOv8 (You Only Look Once, version 8)  
- **Task**: Object Detection  
- **Use Case**: Perception system for self-driving cars  
- **Frameworks**: PyTorch, Ultralytics YOLOv8  

## 📂 Dataset

kaggle inages 

Classes Detected:
- 🚘 Car
- 🚌 Bus
- 🚶 Pedestrian
- 🚦 Traffic light
- 🛑 Stop sign

## 🧪 Sample Results

| Input Image | Detection Output |
|-------------|------------------|
| ![input](examples/input1.jpg) | ![output](examples/output1.jpg) |

## 🚀 How to Run

```bash
# Clone the repo
git clone https://github.com/yourusername/self-driving-yolov8.git
cd self-driving-yolov8

# Install dependencies
pip install -r requirements.txt

# Train or detect
yolo task=detect mode=train model=yolov8n.pt data=your_dataset.yaml epochs=50
yolo task=detect mode=predict model=best.pt source=test_images/
