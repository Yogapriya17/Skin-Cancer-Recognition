# Skin Cancer Recognition using ResNet-50 🧠🩺

This project aims to classify dermoscopic images of skin lesions as **benign** or **malignant** using a deep learning model based on the **ResNet-50** architecture. It provides an assistive tool for early skin cancer detection, leveraging image processing and CNNs for accurate diagnosis.

---

## 📌 Project Highlights

- ✅ Implemented in **Python** using **TensorFlow/Keras**
- ✅ Utilized **ResNet-50** pre-trained model (transfer learning)
- ✅ Dataset includes various dermoscopic images (augmented for training)
- ✅ Classified skin lesions into **benign** and **malignant**
- ✅ Achieved high accuracy and effective validation performance

---
🔍 Project Workflow – Step-by-Step
Problem Definition
The goal of this project is to develop a system that can accurately identify and classify skin lesions as either malignant (cancerous) or benign (non-cancerous) based on dermoscopic images.

1. Dataset Collection

Used the ISIC Archive (International Skin Imaging Collaboration) for dermoscopic images.

Images are labeled with benign or malignant categories.

2. Data Preprocessing

Image Resizing: Images were resized to a standard size (e.g., 224x224) to match the input size required by the ResNet-50 model.

Normalization: Pixel values were normalized to a range of 0-1 to improve the model's performance during training.

Label Encoding: Labels were converted to binary format (0 for benign and 1 for malignant).

3. Data Augmentation: Used techniques such as rotation, flipping, and zooming to artificially increase the dataset and help prevent overfitting.

Model Architecture – ResNet-50

Leveraged ResNet-50, a pre-trained Convolutional Neural Network (CNN) model, using transfer learning.

Removed the final classification layer and added custom layers for binary classification (benign vs. malignant).

Used ReLU activation functions for hidden layers and Sigmoid for the output layer.

4. Model Compilation

Loss function: Binary Cross-Entropy (since it's a binary classification problem).

Optimizer: Adam optimizer to adaptively adjust learning rates.

Metrics: Used Accuracy, Precision, Recall, and F1-Score to evaluate the model’s performance.

5. Model Training

Trained the model on the augmented training dataset while validating it on a separate validation set to monitor performance and overfitting.

Used early stopping to halt training if validation accuracy stopped improving.

Visualized training and validation accuracy and loss curves to ensure that the model was converging properly.

5. Model Evaluation

Evaluated the model on a separate test set that the model had not seen before.

Calculated performance metrics (Accuracy, Precision, Recall, F1-Score) and examined the Confusion Matrix.

6. Saving the Model

Saved the final trained model (resnet50_skin_cancer_model.h5) for future inference or deployment.

📊 Performance Metrics

- ✅ Accuracy: 92%
- ✅ Precision: 90%
- ✅Recall: 94%
- ✅F1-Score: 92%





