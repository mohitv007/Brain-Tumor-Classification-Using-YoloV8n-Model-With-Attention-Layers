# Brain-Tumor-Classification-Using-YoloV8n-Model-With-Attention-Layers
🚀 Overview

This project focuses on improving brain tumor detection from MRI scans using the YOLOv8n architecture enhanced with three powerful attention mechanisms:

CA-Net (Comprehensive Attention Network)

BAM (Balanced Attention Mechanism)

MSAF (Multimodal Split Attention Fusion)

These attention modules significantly boost feature extraction capability—especially for complex medical images—while keeping inference time suitable for real-time clinical applications.

🎯 Objectives

Detect & Classify: Perform multi-class detection of Glioma, Meningioma, and Pituitary tumors from MRI scans.

Enhance: Improve the baseline YOLOv8n model using attention mechanisms tailored for medical image analysis.

Compare: Analyze how contextual attention (CA-Net), detail-enhancing attention (BAM), and multimodal fusion attention (MSAF) affect detection performance.

🏗️ Methodologies Implemented 🔵 CA-Net (Comprehensive Attention Network)

Focus: Multi-scale contextual reasoning + anatomical explainability Benefit:

Captures broader anatomical context

Produces interpretable attention maps

Improves recall on irregular and ambiguous tumor boundaries

🟠 BAM (Balanced Attention Mechanism)

Focus: Balanced channel & spatial refinement inspired by super-resolution Benefit:

Enhances high-frequency details

Improves detection of small or low-contrast lesions

Minimal parameter overhead → great for YOLOv8n

🟣 MSAF (Multimodal Split Attention Fusion)

Focus: Split-attention weighting across MRI modalities (T1, T2, FLAIR) Benefit:

Learns which modality is most important for each tumor

Strong multi-scale representation

Achieved the highest overall mAP scores in experiments

📊 Dataset

Source: Public MRI brain tumor datasets (Kaggle / Figshare)

Modalities: T1, T2, FLAIR (used in MSAF variant)

Preprocessing:

Resized to 640 × 640

Normalized intensities

YOLO-format annotations

Classes:

0 → Glioma

1 → Meningioma

2 → Pituitary

🚀 Installation & Usage 📦 Prerequisites

Python 3.8+

PyTorch (CUDA recommended)

Ultralytics YOLOv8

NumPy, OpenCV, Matplotlib
