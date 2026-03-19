## **1. Project Title**

**Computer Vision Powered Image Search & Object Detection using YOLOv11**

---

## **2. Abstract / Introduction**

This project implements a **YOLOv11-based object detection and visual search system** using deep learning.

Users can upload an image through a **Streamlit web interface**, and the system:

* Detects objects using YOLOv11
* Identifies objects from the COCO dataset
* Displays results with bounding boxes
* Performs fast inference on CPU/GPU

The project demonstrates a complete pipeline from **model inference → web deployment → user interaction**.

---

## **3. Dataset & YOLO Model Details (COCO)**

### **Dataset: COCO 2017**

* 118K training images
* 5K validation images
* 80 object categories

Common classes include:

* Person
* Car
* Dog
* Laptop
* Cup

---

### **YOLOv11 Model**

* Model Used: **yolo11m.pt**
* Pretrained on COCO dataset
* Supports real-time object detection
* High speed and accuracy

---

## **4. Environment Setup**

### **Create Conda Environment**

```bash
conda create -n yolosearch python=3.10 -y
conda activate yolosearch
```

### **Install Dependencies**

```bash
pip install ultralytics
pip install streamlit
pip install opencv-python
pip install numpy
pip install pillow
pip install torch torchvision torchaudio
```

---

## **5. GPU Installation Steps OR CPU Installation Steps**

### **GPU Setup (Recommended)**

1. Install NVIDIA CUDA Toolkit (11.8 recommended)
2. Install cuDNN
3. Install PyTorch with GPU:

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

---

### **CPU Setup**

```bash
pip install torch torchvision torchaudio
```

---

## **6. How to Run in VS Code using Conda**

### **Step 1 — Open Project in VS Code**

Open the project folder in VS Code.

---

### **Step 2 — Activate Environment**

```bash
conda activate yolosearch
```

---

### **Step 3 — Run Application**

```bash
streamlit run app.py
```

---

### **Step 4 — VS Code Tips**

* Select correct Python interpreter
* Use integrated terminal
* Ensure all dependencies are installed

---

## **7. How to Deploy using Streamlit**

Run the application:

```bash
streamlit run app.py
```

### **Features**

* Upload image
* Detect objects using YOLOv11
* Display bounding boxes
* Fast and interactive UI

---

## **8. Output Screenshots**

Include these images inside your repository under `screenshots/`:

* Conda environment activation
* Running Streamlit command
* Streamlit UI in browser
* Detection output with bounding boxes

<img width="1883" height="612" alt="workshop3-1" src="https://github.com/user-attachments/assets/5f62a310-e8bd-4e7d-a9cd-3e9ea8e2fbbb" />
<img width="1787" height="708" alt="Screenshot 2026-03-17 140209" src="https://github.com/user-attachments/assets/209cc6eb-89b4-4885-9dc2-ea6d3823a1ec" />
<img width="1754" height="762" alt="image" src="https://github.com/user-attachments/assets/52824397-8b70-421f-991e-2114be975454" />

<img width="1848" height="948" alt="Screenshot 2026-03-17 140744" src="https://github.com/user-attachments/assets/5f0ca0e6-5669-457b-afb1-777a9afc8e27" />
<img width="1728" height="837" alt="Screenshot 2026-03-17 141028" src="https://github.com/user-attachments/assets/6dfba8aa-c3c0-41d5-b9d4-75abd90fc02e" />

  

---

## **9. Enhancements / Innovations Added**

* Implemented **real-time object detection**
* Built **Streamlit web interface**
* Added **GPU support for faster inference**
* User-friendly UI for image upload
* Modular project structure

---

## **10. Results & Conclusion**

### **Results**

* Accurate object detection on COCO classes
* Fast response time
* Works on both CPU and GPU

---

### **Conclusion**

This project successfully demonstrates a **real-time object detection system** using YOLOv11 with a **Streamlit interface**.

It is scalable, efficient, and suitable for real-world applications such as:

* Surveillance systems
* Smart search engines
* Image-based automation

---

## **11. Repository Structure**

```bash
YOLOV11_IMAGE_SEARCH/
│
├── app.py
├── requirements.txt
├── README.md
├── yolo11m.pt
│
├── screenshots/
│   ├── conda_env.png
│   ├── streamlit_run.png
│   ├── ui.png
│   ├── detection.png
│
├── src/
├── data/
├── configs/
├── test/
```

---

## **12. Requirements**

```txt
ultralytics
streamlit
opencv-python
numpy
pillow
torch
torchvision
torchaudio
```

## Author
KESHAVARTHINI B

## License
This project is for academic purposes.

