# 🏥 Brain Tumor Detection using YOLOv11 (Internship Project)

**Google Colab Implementation** | **[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1k5PrarfEaShn4avfkZY7Rs4qsZSXIiXF#scrollTo=_wrptwN2ocpG)**

## 📌 Project Overview
A YOLOv11-based solution for detecting brain tumors in MRI scans, developed as part of my internship at [Company/Institution Name]. Implemented entirely in Google Colab using PyTorch.

## 🔗 Resources
- **Google Colab Notebook**: [Open Notebook](https://colab.research.google.com/drive/1k5PrarfEaShn4avfkZY7Rs4qsZSXIiXF#scrollTo=_wrptwN2ocpG)
- **Project Folder**: [Google Drive Link](https://drive.google.com/drive/folders/1Ck7hFT1VbBqQZ-yuhLRYw4YqOETe61Lv?usp=sharing)
- **Dataset**: ![Training Sample](train_batch0.jpg)

## 🛠️ Technical Implementation

### 1. Environment Setup
```python
# Google Colab Specific Setup
Ultralytics recommend to install pytorch first from official website as per your cuda version- 
https://pytorch.org/get-started/locally.
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
pip install Ultralytics

### 2. Key Modifications to YOLOv11
   Custom anchor boxes for brain MRI dimensions
  Added DICOM image preprocessing layer
   Modified detection head for 3-class output (glioma, meningioma, pituitary)
