# 🧠 Brain Tumor Detection and Segmentation with YOLOv2 and Medical SAM
This project aims to detect and segment brain tumor regions in MRI images. In this deep learning-based system, tumors are first detected using the YOLOv2 object detection algorithm. The detected regions are then segmented in detail using Medical SAM (Segment Anything Model for Medical Images).

## 📁 Project Structure
📂 Models   
📄 yolovGUI.mlapp  
📄 DeepLearningReport.pdf  

## 👥 Team
This project was developed by a team of five students as part of the Deep Learning course. Each team member trained a different neural network model for object detection.
In this project, I trained the SqueezeNet model and developed the application interface using MATLAB App Designer.

Models used:

- SqueezeNet

- ResNet50

- ResNet18

- VGG16

- MobileNetV2

## 🔍 Methods Used
✅ YOLOv2 (You Only Look Once v2)

- Training was conducted in the MATLAB environment.

- The training data consists of MRI images containing brain tumors.

- The model marks tumor regions with bounding boxes.

✅ Medical SAM (Segment Anything Model for Medical Images)

- Tumor regions detected by bounding boxes are segmented using Medical SAM.

- The segmentation process was also implemented in MATLAB.

- Pixel-level segmentation is applied within each bounding box.

## 🗂️ Dataset
Source: Kaggle - Brain MRI Images for Brain Tumor Detection
Type: Grayscale MRI images

Classes:

- Tumor Present

## 🔧 Data Preprocessing
- Image formats were converted to .jpg.

- All images were resized to 416x416 pixels (required for YOLOv2).

- Bounding boxes were normalized before segmentation.

## 📊 Evaluation Metrics
For YOLOv2:

- Precision

- Recall

- mean Average Precision (mAP)

For Segmentation:

- IoU (Intersection over Union)

- Dice Coefficient

## 📌 Results
- YOLOv2 successfully detected tumors in MRI scans.
- With the integration of Medical SAM, the segmentation of detected tumors was made more precise.
- The model outputs were visually validated and confirmed.

This study demonstrates the effectiveness of a multi-stage deep learning approach in the field of medical image processing.

## 🖼️ Screenshots
Below are some screenshots from the application and training results. These visuals display the graphical user interface, model predictions, and performance metrics obtained during the project.

## 🖥️ Application Main Screen
![Uygulama Ana Ekranı](https://github.com/user-attachments/assets/27945626-b572-4377-a614-b072f720a8a1)

## 📌 Model Selection
![Model Seçimi ](https://github.com/user-attachments/assets/099002ac-7626-4acf-b365-02faabe14499)

## ⬇️ Model Loading
![Model Yükleme](https://github.com/user-attachments/assets/0e53794a-76a9-4998-ac89-08fdf6dd6d5a)

## 🖼️ Image Selection
![Görsel Seçimi](https://github.com/user-attachments/assets/b1b47698-1903-468b-bbc7-6bc3fc263476)

## 📂 Image Upload
![resim yükleme](https://github.com/user-attachments/assets/0d9d726e-bc8e-4a15-860f-b227f075f132)



## 🎯 Detection
![tespit](https://github.com/user-attachments/assets/f411d957-da5b-4bbb-adca-304a74a8e28b)

## 🎨 Segmentation with Medical SAM
![boyama](https://github.com/user-attachments/assets/aaaf9a50-5e7c-46c3-8638-4124ed1b6884)
