# 📌 Classification Models: KNN, Logistic Regression, SVM, and Ensemble Methods

### *Machine Learning & Data Science - ENCS5341*
🚀 **Exploring Key Classification Algorithms for Machine Learning**

---

## 📚 **Project Overview**
This project explores **classification algorithms**, including **K-Nearest Neighbors (KNN), Logistic Regression, Support Vector Machines (SVM), and Ensemble Methods (Boosting & Bagging)**. Using the **Iris dataset**, we analyze the performance of these models across various evaluation metrics.

We compare models based on **accuracy, precision, recall, F1-score, and ROC-AUC**, and optimize them using hyperparameter tuning and cross-validation.

---

## 📂 **Repository Structure**
```
📂 Assignment_3_Classification_Models
│── 📝 README.md (This file)
│── 📝 Report.pdf (Detailed analysis and discussion)
│── 📝 ML_assignment_3_description.pdf (Assignment instructions and requirements)
│── 📁 Codes and datasets (Contains the code and dataset)
│    │── 📊 assignment.ipynb (Jupyter Notebook with code and analysis)
│    │── 📝 dataset.csv (Preprocessed dataset)
```

---

## 🔍 **Dataset Overview**
The dataset used is the **Iris dataset**, consisting of **150 samples and four numerical features**:

| Feature Name         | Description |
|---------------------|-------------|
| `Sepal Length`     | Length of the sepal in cm |
| `Sepal Width`      | Width of the sepal in cm |
| `Petal Length`     | Length of the petal in cm |
| `Petal Width`      | Width of the petal in cm |
| `Species`         | Target variable representing the class of the flower |

The dataset has **three classes**:  
🌸 **Setosa** (0) | 🌿 **Versicolor** (1) | 🌺 **Virginica** (2)

📌 **Note:** The dataset is preprocessed to handle missing values and duplicate samples.

---

## 📊 **Machine Learning Models Implemented**
### **🔹 Part 1: K-Nearest Neighbors (KNN)**
- Implemented **KNN classifier** with **three distance metrics**:
  - ✅ **Euclidean Distance** (Best performance)
  - ✅ **Manhattan Distance**
  - ✅ **Cosine Distance** (Lower accuracy)
- Used **cross-validation** to find the optimal value of **K (number of neighbors)**.
- **Best choice:** **Euclidean Distance with K=3** (100% accuracy).

### **🔹 Part 2: Logistic Regression**
- Implemented Logistic Regression with **L1 (Lasso) and L2 (Ridge) regularization**.
- Hyperparameter tuning for **C (regularization strength)**.
- **Final model achieved 100% accuracy after tuning.**

### **🔹 Part 3: Support Vector Machines (SVM)**
- Implemented **SVM classifier** with three different kernels:
  - ✅ **Linear Kernel**
  - ✅ **Polynomial Kernel**
  - ✅ **Radial Basis Function (RBF) Kernel** (Best performance)
- **RBF Kernel achieved 100% accuracy**, making it the best model for this dataset.

### **🔹 Part 4: Ensemble Methods**
- **Boosting (AdaBoost)** and **Bagging (Random Forest, Bagging Classifier)**
- Compared **Random Forest vs AdaBoost**:
  - ✅ **Random Forest achieved 100% accuracy.**
  - ✅ **AdaBoost performed slightly worse, struggling with Class 1.**

📌 **Final Best Model: Random Forest & RBF SVM (100% accuracy).**

---

## 🛠️ **Technologies Used**
✅ **Python**  
✅ **Pandas, NumPy** (Data Processing)  
✅ **Matplotlib, Seaborn** (Visualization)  
✅ **Scikit-learn** (Machine Learning)  

---

## 📝 **How to Run the Project**
1️⃣ Clone the repository:
```bash
git clone https://github.com/ManarShawahni/Machine-Learning.git
```

2️⃣ Navigate into the project directory:
```bash
cd Machine-Learning/Assignment_3_Classification_Models/Codes and datasets
```

3️⃣ Open Jupyter Notebook:
```bash
jupyter notebook
```
- Open `assignment.ipynb`
- Run each cell sequentially to execute the analysis.

4️⃣ **Alternatively, run Jupyter Notebook in VS Code:**
```bash
code .
```
- Open `assignment.ipynb` in **VS Code**.
- Ensure the **Jupyter extension** is installed:
  - Open **VS Code**.
  - Press **Ctrl + Shift + P**, search for **Extensions: Install Extensions**.
  - Search for **Jupyter** and install it.
- Click on **Run All** to execute the notebook.

5️⃣ **Explore the analysis and modify as needed.**


