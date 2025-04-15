# 🧠 Multi-Defect Detection in PCBs using YOLOv8 + Dash

This project detects **multiple defects** in **Printed Circuit Boards (PCBs)** using the **YOLOv8** object detection model. It features a seamless integration with a **Dash web application** that allows real-time image upload, inference, and visualization of results.

---

## 📌 Key Features

- 🔍 Multi-defect detection on PCB images using YOLOv8
- 🧠 Pre-trained or custom-trained YOLOv8 model
- ⚡ Real-time inference via Dash interface
- 🖼️ Upload PCB images and visualize defects with bounding boxes
- 💡 Easy to customize and extend with new data or models

---

## 🏗️ System Architecture

[ PCB Image Upload ] 
        ↓ 
[ Dash Web App ] 
        ↓ 
[ YOLOv8 Model Inference ] 
        ↓ 
[ Annotated Image Output ]


---

## 🧠 Model: YOLOv8

- Framework: [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)
- Model Used: `YOLOv8n` (can upgrade to `s`, `m`, `l`, or `x`)
- Trained on: **PCB Defect Detection Dataset**
- Supported Defects:
  - Missing Hole
  - Mouse Bite
  - Open Circuit
  - Short
  - Spur
  - Spurious Copper

---

## 📂 Dataset

- Dataset: [PCB Defect Dataset]
- Format: YOLO annotation (images + `.txt` labels)
- Includes training and validation sets

---

## 🖥️ Dash Web Interface

- 📁 Upload PCB images
- 🔍 View predicted defects
- 📌 Display bounding boxes with class labels and confidence scores
- ⚙️ Fast and lightweight web interface

---

## 🗂️ Project Structure

├── app.py # Dash web app ├── detect.py # YOLOv8 inference script ├── models/ │ └── best.pt # Trained YOLOv8 model ├── dataset/ │ └── images/, labels/ # Dataset used for training ├── assets/ │ └── styles.css # (Optional) Custom styles ├── requirements.txt # Dependencies └── README.md

## ✅ Requirements
Python 3.8+

YOLOv8 (ultralytics)

Dash & Plotly

OpenCV, NumPy

## 🚀 Future Enhancements
 Live webcam/video defect detection

 Upload batch images

 Download defect reports (CSV/PDF)

 Model selection toggle from UI

 ## 🙋‍♂️ Contact
📧 njharishkumar@gmail.com
