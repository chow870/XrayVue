# 🩺 ML Tuberculosis Detection using Deep Learning (React + FastAPI)

This project is a **Tuberculosis (TB) detection system** built using a **Vite + React frontend** and **FastAPI backend**. It allows users to upload **chest X-ray images**, processes them using a **CNN model**, and generates a **detailed PDF report** with:
- **Prediction Results**
- **Heatmaps**
- **Evaluation Metrics**

---

## 🚀 Features
- **X-ray Upload**: Users can upload chest X-ray images.
- **TB Prediction**: The CNN model (`my_cnn_model.h5`) predicts TB probability.
- **Grad-CAM Heatmaps**: Highlights areas influencing the prediction.
- **PDF Report Generation**: Contains results, confidence scores, and heatmaps.
- **FastAPI Backend**: Processes images and serves predictions via REST API.

---

## 🛠️ Installation Guide

### 1 Clone the Repository
```sh
git clone https://github.com/yourusername/ml-tb-detection.git
cd ml-tb-detection

2 SETUP BACKEND
cd server
python -m venv venv          # Create a virtual environment
venv\Scripts\activate        # Activate it (Windows PowerShell)
pip install -r requirements.txt  # Install dependencies
uvicorn main:app --reload     # Start FastAPI server

For Linux/macOS:
source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload

3️ Set Up the Frontend (Vite + React)
cd ../client
npm install      # Install dependencies
npm run dev      # Start Vite development server