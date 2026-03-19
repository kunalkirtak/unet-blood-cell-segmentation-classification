# 🧠 Leveraging U-Net for Efficient Blood Cell Segmentation and Classification

![Python](https://img.shields.io/badge/Python-3.9-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 📌 Title

**Leveraging U-Net for Efficient Blood Cell Segmentation and Classification**

---

## 📄 Abstract

Accurate segmentation and classification of blood cells are crucial for the diagnosis of various hematological disorders. Traditional methodologies often rely on manual analysis, which can be time-consuming and subject to human error.

In this study, we introduce **HemoDetect**, an automated system that employs a U-Net architecture for the precise segmentation and classification of red blood cells (RBCs), white blood cells (WBCs), and platelets in microscopic blood images.

The U-Net model was trained on a dataset comprising **360 annotated images**, each paired with ground truth masks in XML format. The training process focused on enhancing segmentation accuracy, resulting in a **validation accuracy of 92.83%** and a **validation loss of 0.1933 over 60 epochs**. The dataset was divided into training and validation subsets using an **80–20 split ratio**, ensuring robust evaluation of model performance.

HemoDetect demonstrates significant advancements in automating blood cell analysis, with the potential to enhance diagnostic efficiency and accuracy in clinical settings. The system effectively segments and classifies blood cells, with output visualizations comprising predicted segmentation masks overlaid on the original images, facilitating clear interpretation of results.

This system significantly enhances the efficiency of blood cell analysis, minimizing the need for manual examination and improving diagnostic capabilities. Future work will investigate the model's adaptability in detecting various hematological conditions, including anemia and leukemia, thereby broadening its clinical relevance.

---

## 🚀 Project Overview

HemoDetect is a deep learning-based system designed to automate the segmentation and classification of blood cells using the **U-Net architecture**.

It identifies and processes:

* 🔴 Red Blood Cells (RBCs)
* ⚪ White Blood Cells (WBCs)
* 🟡 Platelets

The system also performs **automated cell counting**, making it highly useful for medical image analysis.

---

## 🎯 Objectives

* Perform accurate multi-class segmentation of blood cells
* Classify RBCs, WBCs, and platelets
* Automate blood cell counting
* Improve diagnostic efficiency using deep learning

---

## 📊 Dataset

* Source: Roboflow
* Total Images: 360 annotated microscopic images
* Annotation Format: XML masks
* Train-Validation Split: 80% / 20%

---

## ⚙️ Methodology

### 🔹 Pipeline

```
Input Image → Preprocessing → U-Net Model → Segmentation Mask → Cell Counting
```

### 🔹 Preprocessing

* Image resizing
* Normalization
* Mask extraction from annotations

---

## 🧠 U-Net Architecture

The model is based on the **U-Net architecture**, widely used for biomedical image segmentation.

### 🔹 Architecture Components

**1. Encoder (Contracting Path)**

* Convolution layers (Conv2D + ReLU)
* MaxPooling for downsampling
* Feature extraction

**2. Bottleneck**

* Deepest representation of features

**3. Decoder (Expanding Path)**

* UpSampling layers
* Skip connections from encoder
* Precise spatial reconstruction

### 🔹 Why U-Net?

* Works well with small datasets
* High segmentation accuracy
* Preserves spatial details using skip connections

---

## 🧪 Training Details

* Model: U-Net
* Optimizer: Adam
* Epochs: 60
* Dataset Split: 80/20
* Loss Function: (Specify based on your implementation)

---

## 📈 Results

| Metric              | Value      |
| ------------------- | ---------- |
| Validation Accuracy | **92.83%** |
| Validation Loss     | **0.1933** |

### 🔢 Sample Cell Counting Output

```
RBC Count: 10
WBC Count: 1
Platelet Count: 2
```

---

## 🖼️ Output Visualizations

The model generates segmentation masks overlayed on input images:

* Original Image
* Ground Truth Mask
* Predicted Mask

📂 Refer to the `results/` folder for outputs.

---

## ✨ Key Features

* Multi-class segmentation using U-Net
* Automated blood cell counting
* Adaptive threshold-based detection
* High accuracy on medical images
* End-to-end deep learning pipeline

---

## 📁 Project Structure

```
├── hemodetect_unet.ipynb
├── dataset/
├── results/
├── README.md
├── requirements.txt
```

---

## ▶️ How to Run

### 1. Clone the Repository

```
git clone https://github.com/kunalkirtak/unet-blood-cell-segmentation-classification.git
cd unet-blood-cell-segmentation-classification
```

### 2. Install Dependencies

```
pip install -r requirements.txt
```

### 3. Run the Notebook

Open:

```
hemodetect_unet.ipynb
```

in Jupyter Notebook or Google Colab.

---

## 🔮 Future Work

* Detection of diseases such as anemia and leukemia
* Real-time clinical deployment
* Training on larger datasets
* Web-based interface for usability

---

## 📄 Research Contribution

This project focuses on advancing **medical image segmentation using deep learning**, contributing to automated diagnostic systems in healthcare.

---

## 👨‍💻 Author

**Kunal B. Kirtak**
B.Tech Electronics and Computer Science
Shri Ramdeobaba College of Engineering and Management

---

## ⭐ Support

If you find this project useful, consider giving it a ⭐ on GitHub!
