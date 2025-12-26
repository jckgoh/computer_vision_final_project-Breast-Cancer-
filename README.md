# Breast Cancer Image Classification

Overview

This project implements an end-to-end deep learning system for breast cancer image classification using a ResNet50-based convolutional neural network. The system classifies breast cancer images into benign or malignant categories and is designed as a complete prototype consisting of a backend inference API and a web-based frontend interface.

The ResNet50 model is selected for deployment due to its superior performance in experimental evaluation, demonstrating high accuracy and strong generalization capability compared to other architectures.

Computer Vision Final Project/
│
├── backend/            # Deep learning backend (ResNet50 inference)
│   ├── app/
│   │   ├── models/     # Trained ResNet50 model (Git LFS)
│   │   └── ...
│   └── requirements.txt
│
├── frontend/           # React + Vite frontend application
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── .gitignore
├── .gitattributes
└── README.md


# Backend Setup
Requirements
- Python 3.9+
- Virtual environment (recommended)

Installation
cd backend

python -m venv venv

venv\Scripts\activate    # Windows

pip install -r requirements.txt

Run Backend
uvicorn app.main:app --reload

The backend API will be available at:
http://127.0.0.1:8000

# Frontend Setup
Requirements
- Node.js (v18 or later recommended)
- npm

Installation
- cd frontend
- npm install

Run Frontend
- npm run dev

Frontend URL:
- http://localhost:5173

# Model File Management
The trained ResNet50 model is managed using Git Large File Storage (Git LFS) due to GitHub’s file size limitations.

Before running the project after cloning:
git lfs install
git lfs pull

# Technologies Used
- TensorFlow / Keras
- ResNet50 (Transfer Learning)
- Python
- React
- Vite
- Git & Git LFS

# Notes
- The node_modules directory is excluded from the repository and must be generated locally using npm install.
- Only the ResNet50 model is used in the deployed system, as it achieved the best performance during evaluation.
- This repository contains a working prototype intended for academic and demonstrational purposes.

# Authors
- Denzel Malik Ibrahim
- Enrico Navarro Lesmana
- Jacknius
