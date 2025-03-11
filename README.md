# Driver Drowsiness Detection using CNN

## 📌 Project Overview

This project aims to develop a **Driver Drowsiness Detection System** using **Convolutional Neural Networks (CNNs)**. The model processes real-time facial images to determine whether a driver is **awake** or **drowsy**, helping to prevent accidents caused by fatigue.

## 📂 Dataset

- **Name:** [Driver Drowsiness Dataset (DDD)](https://www.kaggle.com/datasets/ismailnasri20/driver-drowsiness-dataset-ddd/data)
- **Description:** A collection of 41,793 facial images labeled as "Drowsy" or "Non Drowsy."
- **Usage:** The dataset is preprocessed and used to train a CNN model for classification.

## 🛠 Installation & Setup

### **1. Clone the Repository**

```bash
git clone https://github.com/yourusername/driver-drowsiness-detection.git
cd driver-drowsiness-detection
```

### **2. Install Dependencies**

Make sure you have Python installed, then install the required packages:

```bash
pip install -r requirements.txt
```

### **3. Download the Dataset**

Download the dataset from [Kaggle](https://www.kaggle.com/datasets/ismailnasri20/driver-drowsiness-dataset-ddd/data) and extract it into the project directory.

## 🚀 How to Run the Project

### **1. Train the Model**

Run the following command to train the CNN model:

```bash
python train.py
```

### **2. Evaluate the Model**

```bash
python evaluate.py
```

### **3. Real-Time Detection**

For real-time webcam-based drowsiness detection:

```bash
python real_time_detection.py
```

## 🏗 Model Architecture

The CNN model consists of:

- **Convolutional Layers:** Extract features from images.
- **Pooling Layers:** Reduce dimensionality while preserving important features.
- **Fully Connected Layers:** Classify images into "Awake" or "Drowsy."
- **Softmax Activation:** Provides probability scores for classification.

## 📊 Performance Metrics

The model is evaluated using:

- **Accuracy**: Achieved 99.94% on the test dataset.
- **Precision, Recall, and F1-score**:
  - Drowsy: **Precision: 99.97%, Recall: 100%**
  - Non-Drowsy: **Precision: 100%, Recall: 99.97%**
  - Overall Accuracy: **99.99%**
- **Confusion Matrix Analysis**: The model performed exceptionally well with near-perfect classification.

## 🔥 Results & Visualization

- **Training Overview:**
  - Model trained for 2 epochs using PyTorch Lightning.
  - Used Adam optimizer with a learning rate of 0.001.
  - Training and validation loss were monitored.
- **Sample Predictions:**
  - Displayed sample images with true vs. predicted labels.
  - Used inverse normalization to visualize images correctly.

