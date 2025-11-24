# YOLO-Based Thermal Cheetah Detection

## Overview
This project implements the YOLO object-detection framework on thermal images of cheetahs.  
The work was completed as part of an academic lab assessment, focusing on practical understanding of detection pipelines, preprocessing, model configuration, and inference on non-RGB datasets.

---

## Objective
- Detect cheetahs in thermal frames using YOLO.
- Study how object detection performs on low-visibility, low-contrast imagery.  
- Build a complete workflow: preprocessing → training → inference → visualization.

---

## Dataset
The dataset used in this project was sourced from Roboflow.  
It contains thermal images of cheetahs annotated for object detection tasks.

- Source: Roboflow Public Datasets (licensed for educational and research use)  
- Format: YOLO-compatible annotations  
- Includes: Thermal frames, bounding-box labels  
- Note: The dataset is not included in this repository due to licensing and size constraints.

---

## Methodology

### 1. Preprocessing
Since the dataset was exported from Roboflow in YOLO format, no manual preprocessing was required.  
Ultralytics YOLO automatically performed resizing, normalization, and image tensor preparation during training.

### 2. Model
- Implemented YOLOv8 using the Ultralytics library.
- Used default YOLOv8 hyperparameters, with minor adjustments as needed.

### 3. Training
- Trained YOLOv8 on the annotated thermal dataset imported from Roboflow.
- Leveraged Ultralytics’ built-in training loop, which logs losses and validation metrics automatically.

### 4. Inference
- Ran inference on unseen thermal frames.
- Obtained bounding boxes and confidence scores.
- Visualized detection outputs for qualitative assessment.

---

## Results
The model successfully detected cheetahs in multiple thermal inputs.  
Performance varied depending on:
- thermal clarity  
- distance from the sensor  
- contrast variation  

---

