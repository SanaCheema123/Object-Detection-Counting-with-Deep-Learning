# 🚗 Object Detection & Vehicle Counting using YOLOv8 and Faster R-CNN

This project focuses on detecting and counting vehicles from aerial and street-level images.  
Initially, **YOLOv8** was used as a baseline model, and later upgraded to **Faster R-CNN**, which delivered significantly higher accuracy, more stable bounding boxes, and improved generalization on unseen images.


## 📌 Dataset Used
Vehicles (Open Images) – Public Roboflow Dataset  
**Link:** https://public.roboflow.com/object-detection/vehicles-openimages/1  

**Dataset Includes:**
- Cars, Buses, Trucks, Motorcycles (Bikes), Ambulances
- Pre-annotated COCO JSON format
- Train / Valid / Test splits with bounding boxes


## 🎯 Project Goals
- Detect multiple vehicle types in images
- Count per-class occurrences (Car, Bike, Bus, Truck, Ambulance)
- Evaluate performance across models
- Run inference on unseen images / direct URL inputs


## 🧠 Models Used

| Model        | Stage     | Accuracy | Behavior on Unseen Images | Notes |
|--------------|------------|----------|----------------------------|-------|
| **YOLOv8**   | Baseline   | 80%+     | Detects & counts well      | Fast inference, good starter |
| **Faster R-CNN (Final)** | Best Model | ~100% | Very accurate & stable | Best precision, ideal for deployment |


## 🚀 Features
- Multi-class vehicle detection
- Per-class counting (Car / Bike / Bus / Truck / Ambulance)
- Works with **local images + external image URLs**
- High-accuracy bounding boxes with enhanced visibility
- Supports unseen images (generalizes well)


## ⚙️ Tech Stack
- Python
- PyTorch
- Torchvision Faster R-CNN
- YOLOv8 (Ultralytics)
- OpenCV, PIL, Matplotlib
- Inference from URL support


## 📊 Results & Visuals

YOLOv8 baseline → Good but inconsistent on unseen images
Faster R-CNN → Much stronger generalization & stability
Bounding boxes improved with dark/outlined edges for clarity

You can add screenshots here:

![Model Output](results/faster_rcnn_output.png)


## 🤝 Collaboration & Contact

If you are interested in improving, deploying, or collaborating on this project:

- **Email:** sanacheema887@gmail.com
- **LinkedIn:** https://www.linkedin.com/in/sanacheema-ml-ai/
- **Available For:** Research | Projects | Freelance | Long-term Collaboration


## ⭐ Acknowledgment

- **Dataset Source:** Vehicles – Open Images (Roboflow Public)  
- **Tools Used:** PyTorch, Torchvision, YOLOv8, Faster R-CNN, OpenCV, PIL  
- Special thanks to the open-source community that made this project possible.


If you want to extend this project, it can be transformed into:

- 🚀 **A Web App** (Streamlit / Gradio interface)  
- 📱 **A Mobile Application** for on-device detection  
- 🎥 **A Real-Time Vehicle Counter** for CCTV, Road Monitoring, or Drone Camera Feed  

Feel free to reach out — I would be happy to help architect and deploy the solution.

## 📌 Setup & Installation

```bash
# Install PyTorch
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121

# Additional dependencies
pip install pycocotools opencv-python matplotlib ultralytics

