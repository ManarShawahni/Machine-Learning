# 📌 Electric Vehicle Data Analysis

### *Machine Learning & Data Science - ENCS5341*

🚗🔋 **Exploring Electric Vehicle Adoption in Washington State**

---

## 📚 **Project Overview**

This project involves analyzing a real-world **Electric Vehicle Population dataset** obtained from [Data.gov](https://catalog.data.gov/dataset/electric-vehicle-population-data). The dataset contains **210,165 entries across 17 features**, providing insights into **EV model popularity, geographic distribution, and trends in EV adoption**.

Through **data cleaning, feature engineering, exploratory data analysis (EDA), and visualization**, we derive meaningful insights from the dataset.

---

## 📂 **Repository Structure**

```
📂 Assignment_1_EV_Data_Analysis
|── 📝 README.md (This file)
|── 📝 Report.pdf (Detailed analysis and discussion)
|── 📝 ML_assignment_1_description.pdf (Contains the assignment instructions and requirments)
|── 📁 Codes and datasets (Contains the codes and the dataset files)
    |── 📊 ML_assignment1.ipynb (Jupyter Notebook with code and analysis)
    |── 📝 dataset.csv

```

---

## 🔍 **Dataset Overview**

The dataset includes **various numerical, categorical, and geographic features** related to electric vehicles registered in **Washington State**.

| Feature Name                         | Description                                               |
| ------------------------------------ | --------------------------------------------------------- |
| `VIN`                                | Unique vehicle identification number                      |
| `Make`                               | Car manufacturer (e.g., Tesla, Nissan)                    |
| `Model`                              | Vehicle model (e.g., Model 3, Leaf)                       |
| `Model Year`                         | Year of manufacture                                       |
| `Electric Range`                     | Estimated electric range (in miles)                       |
| `Clean Alternative Fuel Eligibility` | Whether the vehicle is eligible for clean fuel incentives |
| `County`                             | Registered county                                         |
| `City`                               | Registered city                                           |
| `Latitude/Longitude`                 | Geographic location                                       |

📌 **Data Source:** [Electric Vehicle Population Data](https://catalog.data.gov/dataset/electric-vehicle-population-data)

---

## ⚙️ **Data Processing & Feature Engineering**

### **🔹 Handling Missing Values**

- **91.8% of missing values** are found in the `Legislative District` feature.
- **Solutions:**
  - **Imputation (Mean, Median, Mode)** for numerical and categorical features.
  - **Dropping Rows** where data is missing.

### **🔹 Feature Encoding**

- **One-Hot Encoding** for low-unique categorical features.
- **Label Encoding** for high-unique categorical features.

### **🔹 Normalization**

- **Min-Max Scaling** (0 to 1 range).
- **Z-score Normalization** (centered around 0).

---

## 📈 **Machine Learning & Model Evaluation**

We explored **regression models** to predict **Electric Range** based on vehicle characteristics.

### **🔹 Regression Models**

- **Linear Regression** – Basic approach.
- **Polynomial Regression** – Captures non-linearity.
- **Decision Tree Regression** – Captures complex interactions.

#### 📊 Model Performance:

| Model                     | R² Score | RMSE |
| ------------------------- | -------- | ---- |
| **Linear Regression**     | 0.67     | 12.4 |
| **Polynomial (Degree=3)** | 0.81     | 8.3  |
| **Decision Tree**         | 0.89     | 5.6  |

📌 *The Decision Tree model performed the best in predicting Electric Range.*  

📌 You can see the full analysis in [Report.pdf](./Report.pdf)

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
git clone https://github.com/ManarShawahni/Machine-Learning/tree/main/Assignment_1_EV_Data_Analysis.git
```

2️⃣ Run the Jupyter Notebook at VScode:

```bash
jupyter notebook
```

3️⃣ Open `ML_assignment1.ipynb` and explore the analysis.
