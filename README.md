# DeepXpose: A Transformer-Based System for Deepfake Video Detection

> Senior Graduation Project – Bachelor of Computer Science (Artificial Intelligence), Effat University

## Overview

DeepXpose is an end-to-end deepfake video detection system designed to identify manipulated videos using a transformer-based architecture. The project addresses key challenges in modern deepfake detection, including generalization across datasets, robustness to compression artifacts, and efficient spatio-temporal feature extraction.

The system integrates a complete AI pipeline consisting of video preprocessing, transformer-based model inference, backend APIs, database management, and a web-based user interface.

---

## Motivation

Recent advances in generative AI have made deepfake videos increasingly realistic and difficult to detect. Existing detection methods often struggle with:

- Generalization to unseen manipulation techniques
- Performance degradation on compressed videos
- Capturing long-range temporal inconsistencies

DeepXpose addresses these limitations through the TALL-Swin transformer architecture and an efficient preprocessing pipeline.

---

## Key Features

- Transformer-based deepfake video detection
- TALL-Swin architecture
- Multi-frame video sampling
- Thumbnail-based frame aggregation
- Secure authentication system
- Video upload and automated analysis
- Detection reports
- Full-stack web application
- Modular AI pipeline

---

## Performance Highlights

| Metric | Result |
|---------|--------|
| Validation Accuracy | **92.1%** |
| Test Accuracy | **92.3%** |
| Average Inference Time | **~95 ms/video** |
| GPU Memory Usage | **< 1 GB** |

### Key Findings

- Achieved **92.3%** test accuracy on benchmark datasets.
- Demonstrated strong cross-dataset generalization.
- Reduced overfitting through multi-dataset training.
- Near-real-time inference (~95 ms per video).
- Lightweight deployment with less than **1 GB** GPU memory usage.

  ---

## System Architecture

*Insert your exported System Architecture image here.*

---

## Methodology

The proposed system follows a modular end-to-end pipeline for detecting deepfake videos.

```text
Video Upload
      ↓
Frame Extraction (FFmpeg + OpenCV)
      ↓
Face Detection (MediaPipe / Dlib)
      ↓
Data Cleaning
      ↓
Thumbnail Layout (2×4 TALL)
      ↓
Normalization (224×224)
      ↓
TALL-Swin Transformer
      ↓
Binary Classification
      ↓
Prediction & Confidence Score

---

## Benchmark Datasets

The model was trained and evaluated using publicly available benchmark datasets:

- DeeperForensics-1.0
- Celeb-DF (v2)
- SDFDV

These datasets contain authentic and manipulated videos captured under diverse lighting conditions, compression levels, identities, and manipulation techniques, improving the model's robustness and generalization.

---

## Training Configuration

| Parameter | Value |
|----------|------|
| Backbone | TALL-Swin Transformer |
| Loss Function | Cross-Entropy Loss |
| Optimizer | AdamW |
| Learning Rate | 1 × 10⁻⁴ |
| Input Resolution | 224 × 224 |
| Frames per Sample | 8 |
| Thumbnail Layout | 2 × 4 (TALL) |
---
## Technology Stack

### AI & Machine Learning

- Python
- PyTorch
- Torchvision
- OpenCV
- FFmpeg
- NumPy
- Pandas
- Pillow
- CUDA
- Scikit-learn

### Backend

- Flask
- SQLAlchemy
- JWT Authentication

### Frontend

- React
- JavaScript
- HTML
- CSS
- Bootstrap
- Axios

### Database

- SQLite

---

## Results

| Model | Accuracy |
|---------|----------|
| XceptionNet | 85% |
| EfficientNet-B4 | 89% |
| Swin-B Transformer | 90% |
| **DeepXpose (TALL-Swin)** | **92%** |

The proposed DeepXpose system achieved:

- **92.1% validation accuracy**
- **92.3% test accuracy**
- **~95 ms** average inference time per video
- **< 1 GB** GPU memory usage

The model demonstrated strong generalization across benchmark datasets while maintaining efficient deployment performance.

---
## Project Modules

- Frontend Interface
- Data Preprocessing
- Model Fine-Tuning
- Testing & Evaluation
- Database Management
- Backend API
- Frontend API

---
## Applications

- Digital Forensics
- Law Enforcement Investigations
- Social Media Content Verification
- Journalism & Fact-Checking
- Enterprise Content Moderation
- AI Security
---
## Research Contributions

- Transformer-based deepfake detection
- Spatio-temporal video analysis
- Efficient preprocessing pipeline
- Robust detection across multiple datasets
- End-to-end deployment architecture

---



## Repository Contents

- Project Presentation
- System Overview
- Architecture Diagrams
- Methodology

> Source code is not included in this public repository.

---

## Authors

- Amani Albarazi
- Bushra Alshehri
- Maram Alhusami

Supervisor:
- Dr. Fidaa Abed
- Dr. Passent Elkafrawy

Instructor:
- Dr. Naila Marir

Effat University
Bachelor of Computer Science (Artificial Intelligence)

---

## Citation

If you reference this work, please cite it as:

**DeepXpose: A Transformer-Based System for Deepfake Video Detection**  
Senior Graduation Project, Effat University.
