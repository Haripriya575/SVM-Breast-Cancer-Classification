# SVM Breast Cancer Classification

## 📌 Overview
This project implements the **Support Vector Machine (SVM)** algorithm to classify breast cancer tumors as malignant or benign.  
The workflow includes:
- Loading and exploring the dataset
- Data normalization using `StandardScaler`
- Training SVM with **Linear** and **RBF** kernels
- Hyperparameter tuning using `GridSearchCV`
- Model evaluation with accuracy, classification report, and confusion matrix

---

## 📂 Dataset
- **Name**: Breast Cancer Wisconsin Dataset (from `sklearn.datasets`)
- **Features**: 30 numeric features describing tumor cell nuclei
- **Target**:  
  - 0 = Malignant  
  - 1 = Benign

---

## ⚙️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

---

## 🚀 Steps Performed
1. Imported libraries and loaded dataset
2. Scaled features using `StandardScaler`
3. Split dataset into train and test sets
4. Trained **Linear Kernel SVM** model
5. Trained **RBF Kernel SVM** model
6. Compared accuracies and performance metrics
7. Performed hyperparameter tuning with `GridSearchCV`
8. Plotted confusion matrix for best model

---

## 📊 Results
- **Linear Kernel Accuracy**: ~97%
- **RBF Kernel Accuracy**: ~98% (after tuning)
- **Best Parameters (from GridSearch)**:  
  `{'C': 1, 'gamma': 0.1, 'kernel': 'rbf'}`
- **Classification Report**:
  - High precision and recall for both classes

---

## 📷 Visualizations
- Confusion Matrix heatmap (RBF Kernel)

---

## 📌 How to Run
```bash
# Clone the repository
git clone https://github.com/yourusername/SVM-Breast-Cancer-Classification.git

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Run the notebook
jupyter notebook svm_breast_cancer.ipynb
