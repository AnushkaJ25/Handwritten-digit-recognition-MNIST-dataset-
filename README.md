# Handwritten Digit Recognition using MNIST

## 📌 Overview
This project focuses on **handwritten digit recognition** using the **MNIST dataset**.  
Multiple machine learning models are implemented and compared, including a **Fast KNN algorithm built from scratch**, Support Vector Machines (SVM), and Decision Trees.  
The project also includes **dimensionality reduction using PCA**, detailed **model evaluation**, and a **voting ensemble** for improved performance.

## 📂 Dataset
- **Dataset:** MNIST Handwritten Digits
- **Format:** CSV
- **Classes:** Digits 0–9
- **Features:** 784 pixel values (28×28 grayscale images)

The dataset is already split into:
- `mnist_train.csv`
- `mnist_test.csv`

Each row consists of:
- `label` → actual digit  
- Remaining columns → pixel intensities (0–255)
- 
## ⚙️ Preprocessing Steps
1. Separation of features and labels  
2. Normalization of pixel values to range `[0, 1]`  
3. Dimensionality reduction using **Principal Component Analysis (PCA)**  
4. Visualization of sample images and class distribution  

## 🧠 Models Implemented

### 1. Fast KNN (From Scratch)
- Implemented without using predefined KNN libraries
- Uses Euclidean distance
- Applies majority voting for classification
- Optimized using PCA to reduce computation time

### 2. Support Vector Machine (SVM)
- Linear kernel
- RBF (Gaussian) kernel

### 3. Decision Tree
- Controlled depth and split parameters to avoid overfitting

### 4. Voting Ensemble
- Combines Fast KNN, SVM (RBF), and Decision Tree
- Uses **hard voting** to determine final prediction

## 📊 Model Evaluation
Each model is evaluated using:
- Accuracy score
- Confusion matrix
- Misclassified sample visualization
- Comparative performance analysis

## 📈 Results Summary
| Model | Accuracy |
|------|---------|
| Fast KNN (Scratch) | 97.39% |
| SVM (Linear) | 93.82% |
| SVM (RBF) | 98.52% |
| Decision Tree | 84.42% |
| Voting Ensemble | 97.88% |


## 🖼️ Visualization
- Sample MNIST images
- Confusion matrices for each model
- Visualization of misclassified digits to understand error patterns

## 🛠️ Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
