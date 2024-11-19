# **Energy Load Forecasting using Quantum and Classical Neural Networks**

This repository contains a comprehensive pipeline for energy load forecasting using hybrid Quantum-Classical Neural Networks (QCNN), including classical Convolutional Neural Networks (CNN) for comparison. The project explores state-of-the-art techniques for time-series forecasting, utilizing quantum principles and classical deep learning approaches.

---

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Installation](#installation)
4. [File Structure and Descriptions](#file-structure-and-descriptions)
5. [Usage](#usage)
6. [Visualizations](#visualizations)
7. [Results](#results)
8. [Contributions](#contributions)
9. [License](#license)

---

## **Project Overview**
The primary objective of this project is to forecast energy load using a combination of classical and quantum machine learning approaches. By leveraging the strengths of quantum computing (e.g., superposition, entanglement) and classical deep learning, the project aims to improve forecasting accuracy and computational efficiency.

---

## **Features**
- **Preprocessing**: Cleanses and prepares time-series data for model training.
- **Feature Extraction**: Utilizes Principal Component Analysis (PCA) and other dimensionality reduction techniques.
- **Model Implementations**:
  - Classical CNN.
  - Quantum CNN (QCNN).
  - Hybrid models combining QCNN with LSTM and RNN.
- **Visualization**:
  - Loss and accuracy trends for training and validation across all models.
  - Comparative analysis of model performance.
- **Modular Code**: Organized into multiple Jupyter notebooks for modularity and clarity.

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/username/energy-forecasting.git
   cd energy-forecasting
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   > Note: Ensure your environment supports quantum computing libraries like PennyLane.

3. Place datasets in the `data/` directory.

---

## **File Structure and Descriptions**

### **1. Preprocessing**
- **File**: `preprocessing.ipynb`
- **Description**: Cleans and normalizes raw time-series data. Handles missing values and scales features to improve model performance.

### **2. Feature Extraction**
- **File**: `featureExtraction.ipynb`
- **Description**: Performs feature extraction using PCA to reduce dimensionality, focusing on key features that maximize variance in the data.

### **3. Model Training**
- **CNN Model**:
  - **File**: `cnn.ipynb`
  - **Description**: Implements and trains a classical CNN for energy load forecasting.

- **QCNN Model**:
  - **File**: `QCNN.ipynb`
  - **Description**: Implements a Quantum Convolutional Neural Network leveraging PennyLane and PyTorch for hybrid quantum-classical training.

- **QCNN + LSTM**:
  - **File**: `QCNN_LSTM.ipynb`
  - **Description**: Combines QCNN with Long Short-Term Memory (LSTM) networks for capturing temporal dependencies.

- **QCNN + RNN**:
  - **File**: `QCNN_RNN.ipynb`
  - **Description**: Combines QCNN with Recurrent Neural Networks (RNN) for sequential data analysis.

### **4. Visualizations**
- **QCNN Visualizer**:
  - **File**: `qcnnVisualizer.ipynb`
  - **Description**: Plots training and validation accuracy trends for all quantum-based models, including QCNN, QCNN-LSTM, and QCNN-RNN.

- **CNN Visualizer**:
  - **File**: `cnn_visualizer.ipynb`
  - **Description**: Visualizes training and validation metrics (loss and accuracy) for the CNN model.

### **5. Comparison**
- **File**: `comparisonMatrix.ipynb`
- **Description**: Compares all models in terms of performance metrics (e.g., accuracy, loss) and computational efficiency.

---

## **Usage**
1. Preprocess the data:
   ```bash
   python preprocessing.py
   ```
2. Perform feature extraction:
   ```bash
   python feature_extraction.py
   ```
3. Train models:
   - CNN:
     ```bash
     jupyter notebook cnn.ipynb
     ```
   - CNN:
     ```bash
     jupyter notebook QCNN.ipynb
     ```
   - CNN:
     ```bash
     jupyter notebook QCNN_LSTM.ipynb
     ```
   - CNN:
     ```bash
     jupyter notebook QCNN_RNN.ipynb
     ```
   
4. Visualize results:
   ```bash
   jupyter notebook comparisionMatrix.ipynb
   ```

---

## **Visualizations**
### Example Plots:
1. **Training Loss and Accuracy**:
   - Trends for both training and validation across all models.
2. **Comparison of Models**:
   - Combined plots showing training and validation accuracy for CNN, QCNN, QCNN + LSTM, and QCNN + RNN.
3. **Key Metrics**:
   - Bar charts and performance matrices for final accuracy, loss, and computational efficiency.

---

## **Results**
- **Best Performing Model**: Hybrid RNN-QCNN
- **Observations**:
  - Quantum models showed 98.86% accuracy.
  - Classical CNN achieved 85.63% accuracy.

---

## **Contributions**
Feel free to contribute by:
- Improving model architectures.
- Adding new visualizations or metrics.
- Extending the quantum-based approaches.

---

## **License**
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.