Predictive Analysis of Metro Traffic Using Weather, Holiday, and Environmental Data

# 🚇 Predictive Analysis of Metro Traffic Using Weather, Holiday, and Environmental Data

![Project Banner](2676973a-f407-4751-8df7-feb272d16f35.png)

## 📌 Overview
Urban transportation systems face increasing congestion, impacting operational efficiency and commuter satisfaction.  
This project uses **machine learning** to predict metro traffic volume based on **weather**, **holiday**, and **environmental** factors.  
Accurate predictions can help metro authorities optimize:
- Train frequency  
- Staffing allocation  
- Maintenance scheduling  
- Targeted promotional campaigns  

---

## 📊 Abstract
We combined historical metro traffic data with environmental and holiday information to train **regression** and **classification** models.  
The best results were achieved with **XGBoost**, providing:
- **Regression:** RMSE = 435.95, R² = 0.952  
- **Classification:** Accuracy = 91.24%  

---

## 🎯 Objectives
1. Perform **Exploratory Data Analysis (EDA)** to discover patterns.  
2. Build **regression models** for predicting passenger volume.  
3. Create **classification models** to categorize traffic levels.  
4. Compare model performances to select the most effective one.  

---

## 📂 Dataset
- **Source:** [Kaggle - Indian Metro Data](https://www.kaggle.com/datasets/umairnsr87/indian-metro-data)  
- **Features Include:**
  - Date & time
  - Weather metrics (temperature, rain, visibility)
  - Pollution data
  - Holiday indicators
  - Metro traffic volume

---

## 🛠 Tools & Libraries
- **Python**: Pandas, NumPy, Matplotlib, Seaborn  
- **Machine Learning**: Scikit-learn, XGBoost  
- **Metrics**:
  - Regression: RMSE, MAE, R²  
  - Classification: Accuracy, Precision, Recall, F1-score  

---

## 🔍 Exploratory Data Analysis (Key Findings)
### ⏰ Time-Based Insights
- Morning peak: **6 AM – 8 AM**, Evening peak: **3 PM – 5 PM**
- Weekdays busier than weekends
- Seasonal highs in **March–May** & **October–December**

### 🌦 Weather Insights
- Mild temperatures (0–15°C) increase ridership
- Heavy rainfall reduces travel

### 🌫 Pollution Insights
- Minimal short-term effect on metro usage

---

## 🤖 Models & Results
### Regression Models
| Model                   | RMSE    | MAE     | R²     |
|-------------------------|---------|---------|--------|
| Linear Regression       | 1802.50 | 1579.74 | 0.186  |
| Random Forest Regressor | 463.43  | 262.45  | 0.946  |
| **XGBRegressor**        | **435.95** | **261.79** | **0.952** |

### Classification Models
| Model                   | Accuracy | Precision | Recall | F1-score |
|-------------------------|----------|-----------|--------|----------|
| Random Forest Classifier| 88.43%   | 0.89      | 0.88   | 0.88     |
| SVM                     | 60.34%   | 0.61      | 0.60   | 0.60     |
| **XGBClassifier**       | **91.24%** | **0.91**  | **0.91**| **0.91** |

---

## 📌 Key Insights
- **Time patterns** dominate metro usage.
- **Weather** & **holidays** significantly affect ridership.
- **Pollution** has negligible short-term impact.

---

## ⚠ Limitations
- Dependent on historical data patterns  
- No real-time updates  
- Does not include special events (concerts, strikes, etc.)  
- Limited station-level detail  

---

## 🚀 Future Scope
1. Real-time data integration  
2. Deep learning models (LSTM, Transformers)  
3. Inclusion of special event data  
4. Geospatial station-level analysis  
5. Deployment in a live decision-support dashboard  

---

## 📦 Installation & Usage
---bash
# Clone this repository
git clone https://github.com/yourusername/metro-traffic-prediction.git

# Navigate into the project folder
cd metro-traffic-prediction

# Install dependencies
pip install -r requirements.txt

# Run the main script
python main.py
