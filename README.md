# NO₂ Concentration Forecasting — New Delhi

This project focuses on forecasting **nitrogen dioxide (NO₂) concentrations** in New Delhi **6 hours ahead**, using historical air pollution data and meteorological variables.  
It follows a **Green AI** perspective, leveraging machine learning and deep learning models to support environmental monitoring and public health decision-making.

---

##  Project Objective

The objective is to **anticipate short-term air pollution peaks** in New Delhi in order to:
- help citizens adapt their activities,
- support schools and vulnerable populations,
- assist local authorities in air quality management.

The project combines a **data science pipeline** with an **interactive web application** for accessible and interpretable predictions.

---

## 📊 Dataset

### Air pollution data
- File: `city_hour.csv`
- Hourly measurements of atmospheric pollutants, including NO₂.

### Meteorological data
Meteorological variables are retrieved using the **Open-Meteo API**, including:
- temperature
- relative humidity
- atmospheric pressure
- wind speed
- precipitation

---

## 🧠 Methodology

### Data preparation
- data cleaning and preprocessing
- merging air pollution and meteorological datasets
- feature engineering (temporal variables, lagged NO₂ values)

### Exploratory Data Analysis (EDA)
- analysis of temporal trends
- study of correlations between NO₂ and meteorological variables

---

## 🤖 Modeling Approaches

Several approaches are explored and compared:

### Classical machine learning
- baseline model
- linear regression
- random forest regression

These models capture non-linear relationships between weather conditions and NO₂ levels.

### Deep learning (LSTM)
A **Long Short-Term Memory (LSTM)** network is implemented to explicitly model **temporal dependencies** in NO₂ concentration time series.

The LSTM model:
- uses sequences of past observations as input,
- captures long-term temporal patterns,
- complements classical models by focusing on sequential dynamics.

---

## 📈 Results

The **Random Forest** model achieves strong performance with an **R² score of approximately 0.72**, demonstrating its ability to model complex non-linear relationships.

The **LSTM model** shows promising results for time series forecasting by effectively learning temporal dependencies, highlighting the relevance of deep learning approaches for air pollution prediction.

---

##  Streamlit Application

An interactive **Streamlit web application** is developed to make predictions accessible and easy to interpret.

The application allows users to:
- input recent meteorological conditions,
- provide the latest NO₂ measurements,
- obtain a **6-hour ahead NO₂ prediction**,
- visualize an air quality indicator (good, moderate, or poor).

---

## Libraries Used

- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- tensorflow / keras  
- requests  
- streamlit  
- joblib  

---

##  Possible Improvements

- improve LSTM architecture and hyperparameter tuning
- extend the forecasting horizon
- integrate additional pollutant variables
- deploy the application in a real-time monitoring setting


## Authors

- Léa Hadj-Said
- Faraa Awoyemi
- Lilia Benabdallah
