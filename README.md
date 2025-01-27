# Real-Time-Face-Mask-Detection-System
Overview

This project uses a Convolutional Neural Network (CNN) to demonstrate a real-time Face Mask Detection System. The system is designed to detect individuals wearing or not wearing face masks from live video streams. It combines the power of deep learning and computer vision to ensure efficient and accurate detection, promoting public safety in real-time scenarios.

# Key Features

High Accuracy: Achieves 95% classification accuracy on a dataset of 10,000+ labeled images.

Real-Time Processing: Processes video streams at 20 FPS, ensuring smooth detection.

Efficient Model: Lightweight CNN model (<5MB) suitable for low-resource devices.

Multi-Face Detection: Detects multiple faces simultaneously in live video feeds.

User-Friendly: Displays bounding boxes with labels ("Mask" or "No Mask") and confidence scores.

# Technologies Used

Programming Language: Python

Deep Learning Framework: TensorFlow/Keras, ResNet (ResNet50 or ResNet18 for lighter models)

Computer Vision: OpenCV

Libraries: NumPy, Matplotlib, Seaborn

# Implementation Workflow

**Dataset Preparation**:

Used the Face Mask Detection Dataset.

Split data into training and testing sets (80:20 split).

Preprocessed images to 224x224 resolution for ResNet compatibility.

**Model Architecture**:

Fine-tuned ResNet50 pretrained on ImageNet for mask classification.

Added custom dense layers for binary classification ("Mask" and "No Mask").

Implemented transfer learning to leverage ResNet’s feature extraction capabilities.

**Training**:

Used Adam optimizer with a learning rate of 0.0001 and binary cross-entropy loss.

Applied data augmentation to improve model robustness.

Achieved convergence in 10 epochs with 97% accuracy on the validation set.

**Face Detection and Integration**:

Used OpenCV's DNN module or Haar cascades for face detection.

Cropped face regions and resized them to feed into the ResNet model for mask classification.

**Real-Time Deployment**:

Integrated the system with a webcam or video feed for real-time mask detection.

Displayed bounding boxes and classification labels with confidence scores.

**Output Example**

Bounding boxes and labels for detected faces:

"Mask (Confidence: 96%)"

"No Mask (Confidence: 92%)"

**Screenshot**

![Screenshot 2024-12-18 230135](https://github.com/user-attachments/assets/f637ad6d-91d7-44d5-b4b7-696f47452e31)

![Screenshot 2024-12-18 230404](https://github.com/user-attachments/assets/bcdf004a-259c-4435-9686-49b096b5a546)

**About Me*

👋 I’m Jatin Choudhury, a data science enthusiast skilled in data analytics, visualization, Machine Learning, Neural Networks and storytelling.

📫 Reach me at:

Email: jatinchoudhury419@gmail.com

Phone: +91 9766281487

💼 LinkedIn: https://www.linkedin.com/in/jatin-choudhury/
