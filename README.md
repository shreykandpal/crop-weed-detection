# Crop and Weed Detection using YOLOv8
  An automated computer vision system built to detect and localize **weeds** versus **crops** in field images using a fine-tuned **YOLOv8 Nano** object detector.

# Problem Statement
  In conventional agriculture, farmers often apply blanket herbicide spraying across entire crop fields. This practice wastes expensive agricultural chemicals, damages healthy crops, and contributes to soil and environmental contamination. 

# Solution
  By utilizing object detection on field cameras, a smart spraying system can identify the precise coordinates of weeds in real-time and trigger targeted micro-sprayers, protecting crops while drastically reducing chemical usage.

# Dataset Overview
  **Total Images:** 1,300 RGB field images (512 × 512 resolution).
  **Annotation Format:** YOLO bounding box format.
  **Classes:**
    `0`: **Crop** (Sesame crop — to be protected)
    `1`: **Weed** (Target for herbicide application)
  **Data Split:** 80% Training (1,040 images) and 20% Validation (260 images).

# Methodology & Tech Stack
  **Architecture:** YOLOv8 Nano (`yolov8n.pt`) via Transfer Learning.
  **Environment:** Google Colab (NVIDIA Tesla T4 GPU).
  **Libraries:** Ultralytics, OpenCV, Matplotlib, PyTorch.
  **Training Parameters:**
    * Image Size: `512x512`
    * Batch Size: `16`
    * Epochs: `15`
    * Optimizer: Auto (SGD/AdamW)

# Model Performance & Results

# Visual Detection Results
