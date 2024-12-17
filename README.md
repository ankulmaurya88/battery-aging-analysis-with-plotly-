# Battery Aging Analysis with Plotly

## ✈️ **Overview**
This project analyzes the aging of Lithium-ion (Li-ion) batteries using the **NASA Battery Dataset**. By studying resistance parameters, we visualize the changes in battery health over multiple charge/discharge cycles.

---

## 🔐 **Key Parameters Visualized**
- **Electrolyte Resistance (Re)**
- **Charge Transfer Resistance (Rct)**
- **Battery Impedance (Re + Rct)**

---

## 📊 **Dataset**
The dataset is sourced from [NASA Battery Dataset on Kaggle](https://www.kaggle.com/code/ankulml/battery-aging-analysis-with-plotly).

### **Dataset Information**
| **Profile**              | **Description**                                                                                                                                     |
|---------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| **Charge Profile**        | Constant Current (CC) at **1.5A** up to **4.2V**, followed by Constant Voltage (CV) until current drops to **20mA**.                                |
| **Discharge Profile**     | Discharge conducted at currents of **1-4A** until specific voltage thresholds (**2.7V, 2.5V**, etc.).                                               |
| **Impedance Measurement** | Conducted using **Electrochemical Impedance Spectroscopy (EIS)** across frequencies from **0.1Hz to 5kHz**.                                         |
| **End-of-Life (EOL)**     | Experiments stopped after **30% capacity fade** or other predefined criteria. Some experiments stopped due to software crashes.                     |

---

## ⚙️ **Project Workflow**

### **1. Data Preparation**
- Load the dataset.
- Filter impedance data with non-null values for **Re** and **Rct**.
- Sort the data based on **time**.

### **2. Visualizations**
- **Electrolyte Resistance (Re) vs Time**
- **Charge Transfer Resistance (Rct) vs Time**
- **Combined Plot**: Re, Rct, and Battery Impedance over time.

---

## 🔍 **Visualizations**

### **1. Electrolyte Resistance (Re) vs Time**
- 📌 **Insight**: Shows how **Electrolyte Resistance (Re)** increases with battery aging.
- Higher resistance reflects the internal deterioration of battery components.

### **2. Charge Transfer Resistance (Rct) vs Time**
- 📌 **Insight**: Indicates the **degradation of charge transfer efficiency**.
- Higher Rct leads to reduced energy transfer capability.

### **3. Combined Plot**
- 📌 **Insight**: Displays **Re**, **Rct**, and **Battery Impedance** for a comprehensive view of aging trends.

---

## 🌐 **Technologies Used**
- **Python**
- **Pandas**
- **Plotly**
- **Jupyter Notebook**

---

## 👨‍💼 **How to Run the Project**

1. Clone or download the repository:
   ```bash
   git clone https://github.com/your-username/battery-aging-analysis.git
   ```

2. Place the dataset file (`metadata.csv`) in the project directory.

3. Install dependencies:
   ```bash
   pip install pandas numpy plotly
   ```

4. Run the analysis script in **Jupyter Notebook** or any Python IDE.

---







## ✨ **Insights Gained**

**Electrolyte Resistance (Re)** and **Charge Transfer Resistance (Rct)** both increase over time, indicatingbattery degradation.
- Combined battery impedance reflects overall aging trends, which can help predict **Remaining Useful Life (RUL)**.
- Monitoring these resistance parameters allows for effective **battery health management**.

---









