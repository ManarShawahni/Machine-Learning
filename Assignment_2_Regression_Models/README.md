# 📌 Regression Analysis and Model Selection

### *Machine Learning & Data Science - ENCS5341*

🚗 **Predicting Car Prices Using Regression Models**

---

## 📚 **Project Overview**
This project explores **regression modeling techniques** to predict **car prices** using a dataset from [YallaMotors](https://www.kaggle.com/datasets/ahmedwaelnasef/cars-dataset/data). The dataset consists of **6,310 car listings** with various attributes such as **engine capacity, cylinders, horsepower, top speed, and seats**.

We implemented **linear and nonlinear regression models**, evaluated their performance, and optimized them using **feature selection, regularization, and hyperparameter tuning**.

---

## 📂 **Repository Structure**
```
📂 Assignment_2_Regression_Models
│── 📝 README.md (This file)
│── 📝 Report.pdf (Detailed analysis and discussion)
│── 📝 ML_assignment_2_description.pdf (Assignment instructions and requirements)
│── 📁 Codes and datasets (Contains the code and dataset)
│    │── 📊 ML_assignment2.ipynb (Jupyter Notebook with code and analysis)
│    │── 📝 dataset.csv (Preprocessed dataset)
```

---

## 🔍 **Dataset Overview**
The dataset includes **9 features** extracted from YallaMotors, with key attributes such as:

| Feature Name         | Description |
|---------------------|-------------|
| `Car Name`         | Name and brand of the car |
| `Engine Capacity`  | Engine size in liters |
| `Cylinders`        | Number of cylinders |
| `Horsepower`       | Engine power output |
| `Top Speed`        | Maximum speed of the car |
| `Seats`            | Number of seats available |
| `Country`         | Country of sale |
| `Price`           | Car price in various currencies |

📌 **Note:** Prices were converted to **USD** for consistency.

---

## ⚙️ **Data Preprocessing & Feature Engineering**
### **🔹 Data Cleaning & Handling Missing Values**
- **Converted prices to USD** using exchange rates.
- **Replaced outliers and non-numeric values** with NaN.
- **Filled missing values** using the median.
- **Encoded categorical features** (Brand, Country) using **Label Encoding**.
- **Standardized numerical features** using **StandardScaler**.

📌 The dataset was split into:
✅ **60% Training**  
✅ **20% Validation**  
✅ **20% Test**

---

## 📊 **Exploratory Data Analysis (EDA)**
✔️ **Histograms, Boxplots, and Correlation Matrix** were used to analyze data distribution and detect outliers.  
✔️ **Feature importance analysis** was performed to identify the most relevant attributes for price prediction.

---

## 📈 **Regression Models Implemented**
### **🔹 Linear Models**
1️⃣ **Standard Linear Regression**  
2️⃣ **LASSO (L1 Regularization)**  
3️⃣ **Ridge Regression (L2 Regularization)**  

📌 **Key Findings:**  
- Ridge performed **better than LASSO**, with a lower MSE.
- **LASSO helped with feature selection** by setting some coefficients to zero.

---

### **🔹 Advanced Regression Models**
4️⃣ **Closed-Form Solution for Linear Regression**  
5️⃣ **Gradient Descent for Linear Regression**  

📌 **Comparison:**  
- The **Closed-form solution** performed slightly better.
- **Gradient Descent** converged well but required tuning the learning rate.

---

### **🔹 Nonlinear Models**
6️⃣ **Radial Basis Function (RBF) Kernel Regression (SVR)**  
7️⃣ **Polynomial Regression (Degree 2-10)**  

📌 **Key Findings:**  
- **SVR (RBF Kernel) outperformed all models**, achieving the lowest **MSE of 0.155**.  
- **Polynomial Regression (Degree 3)** also performed well, but higher degrees **(5-10)** led to overfitting.

---

## 🎯 **Model Selection & Optimization**
### **🔹 Feature Selection with Forward Selection**
- **Selected Features:** `Horsepower, Seats, Cylinders, Top Speed, Brand`
- **Reduced MSE to 0.2395**, confirming the importance of selected features.

### **🔹 Regularization Techniques**
- **Ridge Regression (L2) performed better than LASSO**.
- **Best alpha values** found via **Grid Search**:
  - ✅ **Ridge α = 890.215**
  - ✅ **LASSO α = 0.0001**

### **🔹 Hyperparameter Tuning (Grid Search)**
- **Optimized Polynomial Regression Degree = 5** (MSE **0.104**)
- **Best SVR parameters: C = 10, epsilon = 0.1** (MSE **0.137**)

📌 **Final Best Model:** **Polynomial Regression (Degree 5)**

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
cd Machine-Learning/Assignment_2_Regression_Models/Codes and datasets
```

3️⃣ Open Jupyter Notebook:
```bash
jupyter notebook
```
- Open `ML_assignment2.ipynb`
- Run each cell sequentially to execute the analysis.

4️⃣ **Alternatively, run Jupyter Notebook in VS Code:**
```bash
code .
```
- Open `ML_assignment2.ipynb` in **VS Code**.
- Ensure the **Jupyter extension** is installed.
- Install Jupyter Extension in VS Code:
  - Open **VS Code**.
  - Press **Ctrl + Shift + P**, search for **Extensions: Install Extensions**.
  - Search for **Jupyter** and install it.
- Click on **Run All** to execute the notebook.

5️⃣ **Explore the analysis and modify as needed.**
