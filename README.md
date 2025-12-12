# 🌸 Image Preprocessing, Augmentation, and Feature Extraction Using Deep Learning

This project demonstrates an end-to-end image processing pipeline that includes **image uploading, preprocessing, augmentation, dimensionality reduction, and simple neural network training** using Python, OpenCV, NumPy, TensorFlow, and Matplotlib.

The system takes an input image, normalizes it, performs various augmentation techniques, extracts features using Global Average Pooling, trains a basic neural network model, and visualizes the results.

---

## 🚀 Features

### **1. Image Uploading**

* Uses Google Colab’s `files.upload()`
* Automatically detects the uploaded image filename

### **2. Image Preprocessing**

* Converts to grayscale
* Normalizes pixel values to binary format (0 and 1)
* Resizes image to **128×128**

### **3. Data Augmentation**

The pipeline applies multiple augmentations:

* Rotation (90° and 60°)
* Horizontal flip
* Vertical flip
* Zoom-in
* Brightness enhancement
* Gaussian blur

### **4. Deep Learning Model**

A simple fully connected neural network is used:

* Flatten → Dense → ReLU layers
* Outputs dummy 10-class softmax for demonstration

### **5. Feature Extraction**

A secondary model uses:

* **Global Average Pooling (GAP)**
  to reduce image dimensions into a compact feature vector.

### **6. Training Visualization**

The project plots:

* **Training loss curve across epochs**

### **7. Visualization of Images**

Displays:

* Original image
* Preprocessed (normalized) image
* All augmented versions

---

## 🛠 Technologies Used

| Library/Tool           | Purpose                         |
| ---------------------- | ------------------------------- |
| **Python**             | Main programming language       |
| **OpenCV**             | Image processing & augmentation |
| **NumPy**              | Numerical computations          |
| **TensorFlow / Keras** | Deep learning models            |
| **Matplotlib**         | Visualization & plotting        |
| **PIL**                | Image loading                   |

---

## 📁 Project Structure

```
├── Upload Image
├── Preprocessing (grayscale & normalization)
├── Augmentation Functions
├── Neural Network Model
├── Feature Extraction Model
├── Training & Loss Plot
└── Visualization of Results
```

---

## 📌 How to Run the Code (Google Colab)

1. Upload your image:

   ```python
   from google.colab import files
   uploaded = files.upload()
   ```
2. The filename is automatically captured:

   ```python
   img_path = list(uploaded.keys())[0]
   ```
3. Run each cell to complete preprocessing, augmentation, feature extraction, and training.

---

## 📷 Sample Augmentations

The code generates the following outputs:

* Normalized Image
* Rotated Images
* Flipped Images
* Zoomed Image
* Brightness Adjusted Image
* Blurred Image

All images are displayed using Matplotlib.

---

## 📈 Model Performance

A simple neural network is trained for **10 dummy epochs**, and the **loss curve** is plotted to demonstrate training behavior.

---

## 🎯 Applications

This project can be extended for:

* Image classification
* Image recognition
* Dataset augmentation
* Feature extraction for ML models
* Preprocessing pipeline for custom datasets


