# CAD to VR – 2D Image to 3D Model Reconstruction

<div align="center">

# 🚀 CAD to VR
### Transforming 2D Images into Interactive 3D Models using AI & Computer Vision

</div>

---

## 📌 Overview

CAD to VR is an AI-powered 3D reconstruction system that converts a single 2D image into an interactive 3D model.

The project combines:

- OpenCV for image preprocessing
- MiDaS for monocular depth estimation
- Open3D for point cloud & mesh generation
- Blender for mesh refinement
- Flask for the web interface

This system demonstrates how Deep Learning and Computer Vision can reconstruct meaningful 3D structures from ordinary images.

---

# ✨ Features

- Upload JPG/PNG images
- AI-powered depth estimation
- Point cloud generation
- Poisson mesh reconstruction
- Adjustable mesh quality (5K–40K faces)
- Interactive Flask web interface
- OBJ/PLY export support
- Real-time 3D preview
- Blender mesh refinement

---

# 🧠 Pipeline

```text
Input Image
     ↓
OpenCV Preprocessing
     ↓
MiDaS Depth Estimation
     ↓
Depth Map Generation
     ↓
Open3D Point Cloud Creation
     ↓
Poisson Surface Reconstruction
     ↓
Blender Mesh Refinement
     ↓
Final 3D Model (.OBJ/.PLY)
```

---

# 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| Language | Python |
| Frontend | HTML, CSS, JavaScript |
| Backend | Flask |
| AI Model | MiDaS (PyTorch) |
| Computer Vision | OpenCV |
| 3D Processing | Open3D |
| Rendering | Blender |
| Numerical Computing | NumPy |

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/CAD-to-VR.git
cd CAD-to-VR
```

---

## 2️⃣ Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux / Mac

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Project

```bash
python app.py
```

Open browser:

```bash
http://127.0.0.1:5000
```

---

# 📸 Screenshots

## Web Interface

<img width="413" height="197" alt="image" src="https://github.com/user-attachments/assets/1754fab2-430c-4c5c-8a7c-d945607299d9" />


# 🔍 Core Modules

## 🔹 Image Preprocessing

- BGR → RGB conversion
- Bilateral filtering
- Noise reduction
- Histogram equalization

Implemented using OpenCV.

---

## 🔹 Depth Estimation

MiDaS predicts relative depth from a single RGB image using a transformer-based architecture.

Features:
- Vision Transformer backbone
- Dense depth prediction
- High-quality monocular depth estimation

---

## 🔹 Point Cloud Generation

Depth map pixels are converted into 3D coordinates using camera projection equations.

Implemented using Open3D.

---

## 🔹 Mesh Reconstruction

- Surface normal estimation
- Poisson reconstruction
- Mesh smoothing
- Face optimization

---

# 📊 Performance

| Face Count | Quality | Speed |
|------------|---------|-------|
| 5K | Fast | ~4 sec |
| 10K | Medium | ~7 sec |
| 20K | High | ~12 sec |
| 40K | Ultra | ~20 sec |

---
