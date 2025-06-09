# ⚡ **PowerPulse: Household Energy Usage Forecast**

---

## 🎯 **Project Overview**

**PowerPulse** is a machine learning project aimed at **predicting household energy consumption** using historical power usage data.  
By analyzing over **2 million minute-wise observations**, we gain actionable insights into usage patterns and develop highly accurate forecasting models.  
This helps **households reduce bills** and enables **energy providers to manage demand** more efficiently.

---

## 📂 **Dataset**

- **Source**: *Individual Household Electric Power Consumption Dataset*
- **Features**:
  - 🔌 Global active power
  - 💡 Global reactive power
  - ⚡ Voltage
  - 🔥 Global intensity
  - 🍽️ Sub_metering_1
  - 🧺 Sub_metering_2
  - 🚿 Sub_metering_3
  - 📅 Date and Time

---

## 🛠️ **Tools and Libraries**

- 🐍 **Python**
- 📝 **pandas** and **numpy** for data cleaning and analysis
- 📊 **matplotlib** and **seaborn** for visualization
- 🤖 **scikit-learn** for machine learning

---

## 🔍 **Steps Followed**

### 🧹 **Data Loading & Cleaning**
- Replaced missing `?` entries with `NaN`, converted data types, and combined **Date** and **Time** columns.

### 📈 **EDA (Exploratory Data Analysis)**
- Visualized daily energy usage trends.
- Analyzed feature distributions and correlations.

### ⚙️ **Feature Engineering**
- Extracted time-based features like `hour`, `weekday`, `weekend`.
- Calculated **total sub-meter usage** and removed data leakage from target-derived features.

### 🤖 **Model Building**
- Trained and evaluated three powerful regression models:
  - **Linear Regression**
  - **Random Forest Regressor**
  - **Gradient Boosting Regressor**

### 🧪 **Model Evaluation**
- Compared models using **RMSE**, **MAE**, and **R²** metrics.

### 🎨 **Visualization**
- Created **Actual vs Predicted** plots.
- Visualized **Feature Importance**.

---

## 🏆 **Key Results**

| 🚀 Model                     | 🎯 RMSE  | 📉 MAE  | 📊 R² Score |
|------------------------------|----------|---------|-------------|
| Linear Regression            | 0.0403   | 0.0258  | 0.9986      |
| Random Forest Regressor      | **0.0289** | **0.0160** | **0.9993**   |
| Gradient Boosting Regressor  | 0.0341   | 0.0214  | 0.9990      |

✅ **Best Model**: **Random Forest Regressor** – with the highest accuracy and lowest error.

---

## 💡 **Key Insights**

- ⚡ Household energy usage follows predictable daily and seasonal patterns.
- 🔍 Sub-metering data reveals high variability—some appliances are used heavily, others rarely.
- 🔌 Voltage is stable (normal distribution around 240V), indicating a healthy power supply.
- 🔥 `Global_intensity` emerged as the most important feature in predicting overall energy consumption.

---

## 🚀 **How to Run**

1️⃣ **Clone this repository:**
```bash
git clone https://github.com/<your_username>/PowerPulse-Household-Energy-Usage-Forecast.git

2️⃣ Install required libraries:
pip install -r requirements.txt
3️⃣ Run the Jupyter Notebook:
jupyter notebook PowerPulse-Household-Energy-Usage-Forecast.ipynb
