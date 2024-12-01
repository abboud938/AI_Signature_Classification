# AI Signature Classification

An AI-powered solution for detecting and classifying handwritten signatures from images. This project combines multiple stages, including object detection, denoising, and classification, to identify signatures accurately.

## Features
- **Signature Detection**: Utilizes a YOLO model to detect signatures in scanned documents.
- **Denoising**: Enhances the quality of detected signature regions using a denoising autoencoder.
- **Signature Classification**: Employs a CNN for feature extraction and Random Forest for classification.

## Project Workflow
1. **YOLO Detection**:
   - Detects the signature bounding boxes in scanned document images.
   - Outputs the cropped signature regions.
    ![YOLO Training Result](yolo/result.png)

2. **Denoising**:
   - Cleans and enhances the extracted signature regions for better classification accuracy.
   ![Denoising Autoencoder Training Result](signature_denoising/result.png)

3. **Classification**:
   - A Convolutional Neural Network (CNN) extracts features.
   - A Random Forest (RF) classifier predicts the signature owner.


