# Anomaly Detection In CCTV Footage

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN%2FAutoencoders-orange)
![Status](https://img.shields.io/badge/Status-Active-green)

A Machine Learning project designed to automatically detect anomalies (such as accidents, fighting, robbery, or other unusual activities) in CCTV surveillance footage. This system aims to reduce the need for manual monitoring by flagging suspicious events in real-time or from recorded video.

## 📋 Table of Contents
- [About the Project](#about-the-project)
- [Features](#features)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [Contact](#contact)

## 🧐 About the Project
Surveillance cameras are everywhere, but monitoring them 24/7 is impossible for humans. This project utilizes **Deep Learning** and **Computer Vision** techniques to analyze video frames and detect deviations from normal patterns.

The model learns "normal" behavior from a training dataset and flags any significant deviation as an "anomaly."

**Key Use Cases:**
* Security monitoring (theft/fighting detection).
* Traffic monitoring (accident detection).
* Industrial safety.

## ✨ Features
* **Video Preprocessing:** Frame extraction, resizing, and normalization.
* **Anomaly Detection Model:** Uses [Insert Model Architecture, e.g., Convolutional Autoencoder / CNN-LSTM / C3D] to learn spatiotemporal features.
* **Real-time Alerting:** (Optional) Flags frames where the reconstruction error exceeds a threshold.
* **Visualization:** Plots anomaly scores over time for analyzed videos.

## 📂 Dataset
This project is compatible with standard anomaly detection datasets. You can use:
1.  **UCSD Pedestrian Dataset** (Ped1/Ped2)
2.  **CUHK Avenue Dataset**
3.  **ShanghaiTech Campus Dataset**
4.  *Or your own custom CCTV footage.*

> **Note:** Please place your dataset in the `dataset/` directory before running the training script.

## 🛠 Technologies Used
* **Programming Language:** Python
* **Libraries:**
    * TensorFlow / Keras (or PyTorch)
    * OpenCV (cv2)
    * NumPy & Pandas
    * Matplotlib (for visualization)
    * Scikit-learn

## 🚀 Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/DeMoN-7/Anomaly-Detection-In-CCTV-Footage.git](https://github.com/DeMoN-7/Anomaly-Detection-In-CCTV-Footage.git)
    cd Anomaly-Detection-In-CCTV-Footage
    ```

2.  **Create a virtual environment (Recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```
    temp

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## 💻 Usage

### 1. Training the Model
To train the model on your dataset, run the training notebook or script:
```bash
python train.py
# OR open the Jupyter Notebook
jupyter notebook Anomaly_Detection.ipynb
