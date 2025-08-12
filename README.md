Predictive Analysis of Metro Traffic Using Weather, Holiday, and Environmental Data

📌 Overview
Urban transportation systems face growing congestion challenges, impacting both operational efficiency and commuter satisfaction. This project applies Machine Learning to forecast metro traffic volume using weather, holiday, and environmental data. The insights can help authorities optimize train frequency, allocate resources effectively, and improve commuter experience.

📊 Abstract
Accurate metro traffic prediction allows for:

Optimized train schedules

Improved staffing allocation

Reduced delays & congestion

Targeted promotional campaigns

We combined historical metro traffic data with environmental factors and holidays. Multiple regression and classification models were tested, with XGBoost models achieving the best results.

🎯 Objectives
Perform EDA to identify traffic patterns.

Build regression models to predict passenger volume.

Develop classification models to categorize traffic levels.

Compare performance and provide actionable recommendations.

📂 Dataset
Source: Kaggle - Indian Metro Data

Features include:

Date & time

Weather metrics (temperature, rain, visibility)

Pollution data

Holiday indicators

Metro traffic volume

🛠 Tools & Libraries
Python: Pandas, NumPy, Matplotlib, Seaborn

ML Frameworks: Scikit-learn, XGBoost

Evaluation Metrics:

Regression: RMSE, MAE, R²

Classification: Accuracy, Precision, Recall, F1-score

🔍 Exploratory Data Analysis (EDA)
Time-Based Insights
Morning peak: 6 AM – 8 AM, Evening peak: 3 PM – 5 PM

Weekdays busier than weekends

Seasonal highs in March–May & Oct–Dec

Weather Insights
Mild temperatures (0–15°C) increase ridership

Heavy rainfall reduces travel

Pollution Insights
Minimal short-term effect on metro usage

🤖 Models & Results
Regression
Model	RMSE	MAE	R²
Linear Regression	1802.5	1579.7	0.186
Random Forest Regressor	463.4	262.4	0.946
XGBRegressor	435.9	261.8	0.952

Classification
Model	Accuracy	Precision	Recall	F1-score
Random Forest Classifier	88.43%	0.89	0.88	0.88
SVM	60.34%	0.61	0.60	0.60
XGBClassifier	91.24%	0.91	0.91	0.91

📌 Key Insights
Time-based patterns dominate metro usage.

Weather & holidays significantly impact ridership.

Pollution levels show negligible short-term effect.

⚠ Limitations
Dependence on historical data patterns

Lack of real-time adaptation

No inclusion of external events (concerts, strikes, etc.)

Limited station-level granularity

🚀 Future Scope
Real-time data integration

Deep learning models (LSTM, Transformers)

Inclusion of external event data

Geospatial station-level analysis

Deployment in decision-support dashboards

📚 References
Kaggle Dataset

Scikit-learn Documentation

XGBoost Documentation

