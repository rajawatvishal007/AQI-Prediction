# AQI-Prediction
AQI Prediction using Machine Learning An end-to-end ML project designed to predict Air Quality Index (AQI) based on historical weather and atmospheric data. Developed using Python, Scikit-Learn, and Pandas, this repository features data preprocessing, feature engineering, and model evaluation to provide accurate environmental insights.
AQI Prediction and Analysis in Major Indian Cities

Live Dashboard
Access the interactive dashboard here:https://nonmenacing-kelli-unplundered.ngrok-free.dev/
Project Overview
This project performs an end-to-end analysis of air quality data across 10 major Indian cities, including Delhi, Mumbai, Kolkata, and Gurugram. The goal is to categorize the Air Quality Index (AQI) into six levels (Good to Severe) based on pollutant concentrations using advanced machine learning techniques.

Key Insights from EDA
Primary Drivers: PM2.5 and PM10 were identified as the most critical pollutants influencing AQI levels.
Regional Disparities: Severe pollution events are most frequently recorded in Delhi and Gurugram, whereas cities like Thiruvananthapuram and Amaravati maintain cleaner air.
Seasonality: Analysis shows high annual volatility in AQI, largely driven by seasonal shifts.

Technical Implementation
Data Preprocessing
Missing Value Treatment: Numerical pollutants were imputed using Median Imputation to remain robust against extreme outliers (e.g., spikes during Diwali or dust storms).
Encoding: Categorical variables like "City" and the "AQI Bucket" target were transformed using Label Encoding for model compatibility.

Machine Learning Models
Three models were rigorously tested for classification performance:
Random Forest Classifier: The top-performing model with 93.5% accuracy.
XGBoost: A highly efficient gradient boosting framework achieving 99.95% training accuracy.
K-Nearest Neighbors (KNN): Used as a baseline non-parametric classifier.
Main Dashboard
<img width="1527" height="695" alt="image" src="https://github.com/user-attachments/assets/a8b29b61-a1cf-4a7e-8733-2801e06f4c6b" />
Model Prediction
<img width="1781" height="790" alt="image" src="https://github.com/user-attachments/assets/b67184f5-ff42-4ea3-a1f0-5fa1afe80d62" />
Pollutant Correlation
<img width="940" height="370" alt="image" src="https://github.com/user-attachments/assets/79c3e85c-5ffc-43ce-9986-719ff9cf195c" />
City-wise Distribution
<img width="969" height="382" alt="image" src="https://github.com/user-attachments/assets/7076db51-e755-4168-8e82-9bdb20ef1eb2" />
Model Accuracy
<img width="991" height="391" alt="image" src="https://github.com/user-attachments/assets/f82ac04b-ffb7-44f0-8af2-dce223bed057" />

data/               # CSV datasets for 10 Indian cities
notebooks/          # Jupyter notebooks for EDA and Model Training
app.py              # Streamlit dashboard source code
model.pkl           # Pre-trained Random Forest model
requirements.txt    # List of dependencies
README.md           # Project documentation

Installation & Usage
Clone the Repo:
git clone https://github.com/your-username/AQI-prediction.git

Install Dependencies:
pip install -r requirements.txt

Run the Dashboard:
streamlit run app.py

Requirements.txt
Create a file named requirements.txt in your root folder and add the following:
streamlit
pandas
numpy
scikit-learn
plotly
matplotlib
seaborn
xgboost









