# Rice Crop Stress Prediction

### Early Prediction and Classification of Rice Crop Stress Using Satellite and Weather Data

## Overview

Rice Crop Stress Prediction is a machine learning project designed to analyse environmental and agricultural parameters to identify and classify rice crop stress at the district level in Andhra Pradesh, India.

The project uses satellite-derived vegetation indices, land surface temperature, soil moisture and meteorological data to study the relationship between environmental conditions and crop stress.

The primary objective is to develop a data-driven approach for identifying potential crop stress conditions ahead of harvest, supporting early agricultural risk assessment and informed decision-making.

## Objectives

- Analyse historical rice crop and environmental data across districts of Andhra Pradesh.
- Identify important environmental factors associated with rice crop stress.
- Develop machine learning models to classify crop stress levels.
- Evaluate model performance using year-based validation and testing.
- Understand the contribution of individual environmental parameters using explainable AI techniques.
- Visualise the geographical distribution of crop stress across districts.

## Study Area and Dataset

- **Study Area:** Rice-growing districts of Andhra Pradesh, India.
- **Study Period:** 2018–2025.
- **Data Frequency:** Monthly observations.
- **Geographical Level:** District-level analysis.
- **Crop Seasons:** Kharif and Rabi/Summer.

The dataset combines satellite-derived, meteorological and agricultural variables to analyse crop conditions over time.

## Environmental Parameters

| Category | Parameters |
|---|---|
| Vegetation Indices | NDVI, EVI |
| Temperature | Land Surface Temperature (LST), Maximum Temperature, Minimum Temperature |
| Soil Conditions | Soil Moisture, Water Availability |
| Weather | Rainfall, Relative Humidity, Wind Speed |
| Evapotranspiration | Evapotranspiration (ET) |
| Temporal Features | Year, Month, Crop Season |
| Derived Features | Lagged environmental variables, temperature range and crop stress index |

## Crop Stress Classification

The project considers three crop stress categories:

1. **Normal:** Conditions indicating relatively healthy crop growth.
2. **Moderate Stress:** Conditions indicating potential environmental stress affecting crop development.
3. **Severe Stress:** Conditions indicating relatively high levels of crop stress.

The classification target is based on the project's harvest stress labels.

## Methodology

The project follows a structured machine learning workflow:

1. **Data Collection:** Obtain historical satellite, weather and agricultural information.
2. **Data Preprocessing:** Clean datasets, handle missing values and organise observations by district, year and crop season.
3. **Feature Engineering:** Generate derived environmental variables and historical lag features to capture temporal patterns.
4. **Exploratory Data Analysis:** Examine environmental trends, feature distributions and relationships with crop stress.
5. **Model Development:** Develop and evaluate machine learning approaches for crop stress classification.
6. **Model Validation:** Use historical years for training and a later year for validation.
7. **Model Testing:** Evaluate generalisation using a separate year-based test dataset.
8. **Explainability:** Apply SHAP-based analysis to understand the contribution of environmental features.
9. **Visualisation:** Generate analytical plots and district-level crop stress maps.

## Machine Learning Models

The project explores the following classification approaches:

- **Logistic Regression:** Baseline classification model.
- **Random Forest:** Ensemble learning model that combines multiple decision trees.
- **XGBoost:** Gradient-boosted decision tree model for classification.
- **LSTM:** A recurrent neural network approach explored for capturing temporal patterns in agricultural data.

## Model Evaluation

Model performance is examined using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Class-wise classification reports

The project uses year-based evaluation to examine model performance on observations from years not used for training.

## Explainable AI

SHAP (SHapley Additive exPlanations) is used to interpret machine learning predictions.

It helps to:

- Identify influential environmental parameters.
- Understand the contribution of individual features.
- Compare the importance of environmental variables.
- Improve the interpretability of model predictions.

## Visualisation and Analysis

The project includes:

- Environmental parameter analysis.
- Crop stress distribution across districts.
- Actual versus predicted stress comparisons.
- Confusion matrices and classification reports.
- SHAP feature importance analysis.
- Geographical visualisation of crop stress across Andhra Pradesh.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Primary programming language |
| Google Colab | Development and execution environment |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib | Data visualisation |
| Scikit-learn | Machine learning and evaluation |
| XGBoost | Gradient boosting classification |
| TensorFlow / Keras | LSTM experimentation |
| SHAP | Model explainability |
| GeoPandas | Geospatial data processing |

## Project Structure

```text
Rice-Crop-Stress-Prediction/
│
├── RiceStressPrediction.ipynb
│
├── README.md
│
└── [Additional datasets and resources,
    if included in the repository]
```

## How to Run

The project is developed using Google Colab.

1. Clone or download this repository.
2. Open `RiceStressPrediction.ipynb` in Google Colab.
3. Install the required dependencies, if not already available.
4. Configure access to the required datasets and Google Drive resources.
5. Execute the notebook cells sequentially.
6. Review the generated model evaluation results, visualisations and crop stress analysis.

## Future Enhancements

- Integrate real-time satellite and weather data.
- Improve temporal modelling for earlier crop stress prediction.
- Expand the analysis to additional rice-growing states.
- Develop a web-based dashboard for district-level crop stress monitoring.
- Integrate automated alerts for districts experiencing severe crop stress.
- Validate predictions using independent ground-level agricultural observations.

## Disclaimer

This project is intended for academic and research purposes. Model predictions depend on the quality, coverage and reliability of the input data. Further validation using independent ground observations is necessary before applying the predictions to real-world agricultural decision-making.

## Author

**Akshitha Gandhi S**

B.E. Computer Science and Engineering

GitHub: [@Akshitha1808](https://github.com/Akshitha1808)

---

*An academic machine learning project focused on data-driven agricultural monitoring and early rice crop stress assessment.*
