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

1️⃣ Clone the repository:

```bash
git clone https://github.com/ManarShawahni/Machine-Learning.git
```

2️⃣ Navigate into the project directory:

```bash
cd Machine-Learning/Assignment_1_EV_Data_Analysis/Codes and datasets
```

3️⃣ Run the Jupyter Notebook:

```bash
jupyter notebook
```
- This will open a Jupyter Notebook interface in your browser.

- Navigate to ML_assignment1.ipynb and open it.

- Run each cell sequentially to execute the analysis.
  

4️⃣ Alternatively, run Jupyter Notebook in VS Code:

```bash
cd .\Assignment_1_EV_Data_Analysis\
```
```bash
cd '.\Codes and datasets\'
```
```bash
code .
```
- Then, open the `ML_assignment1.ipynb` file in **VS Code**.
- Ensure the **Jupyter extension** is installed.
  
    - Open VS Code.

    - Press Ctrl + Shift + P and search for Extensions: Install Extensions.

    - Search for Jupyter and install it.
      
- Click on **Run All** to execute the cells.

5️⃣ Explore the analysis and modify as needed.
