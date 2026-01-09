# NO₂ Concentration Forecasting — New Delhi

This project focuses on predicting **nitrogen dioxide (NO₂) concentrations** in New Delhi **6 hours ahead**, using historical air pollution data combined with meteorological variables.  
It follows a **Green AI** approach, aiming to leverage machine learning to support public health and environmental decision-making.

---

##  Project Objective

The objective is to **anticipate pollution peaks** in New Delhi in order to help:
- citizens adapt their outdoor activities,
- schools and vulnerable populations take preventive measures,
- local authorities improve air quality management.

The project combines a **data science pipeline** with an **interactive web application** for easy access to predictions.

---

##  Dataset

### Air pollution data
- Main file: `city_hour.csv`
- Hourly air pollutant measurements, including NO₂ concentrations.

### Meteorological data
Weather variables are retrieved using the **Open-Meteo API**, including:
- temperature
- relative humidity
- atmospheric pressure
- wind speed
- precipitation

---

##  Methodology

### Data processing
- data cleaning and preprocessing
- merging air pollution and meteorological datasets
- feature engineering (temporal variables, lagged NO₂ values)

### Exploratory Data Analysis (EDA)
- analysis of temporal patterns
- study of correlations between NO₂ and weather variables

### Modeling
Several models are trained and compared:
- baseline model
- linear regression
- random forest regression

---

##  Results

The **Random Forest** model achieves the best performance, with an **R² score of approximately 0.72**, demonstrating a strong ability to capture **non-linear relationships** between meteorological variables and NO₂ concentrations.

---

##  Streamlit Application

An interactive **Streamlit web application** is developed to make the predictions accessible and easy to interpret.

The application allows users to:
- input recent meteorological conditions
- provide the latest NO₂ measurements
- obtain a **6-hour ahead NO₂ prediction**
- visualize an air quality indicator (good, moderate, or poor)

---

##  Libraries Used

- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- requests  
- streamlit  
- joblib  

---

## Authors

- Léa Hadj-Said
- Faraa Awoyemi
- Lilia Benabdallah
