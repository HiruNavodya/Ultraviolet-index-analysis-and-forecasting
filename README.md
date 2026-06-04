# Ultraviolet-index-analysis-and-forecasting
Ultraviolet index analysis and forecasting using advanced modelling approaches for different climatic zones in Sri Lanka

https://drive.google.com/drive/folders/1lmoDtHg0reGsEPABrt4s2ysQvKZVdprU?usp=sharing


NASA POWER Data Retrieval Procedure
Data Source

Hourly Ultraviolet Index (UVI) data were obtained from the NASA Prediction of Worldwide Energy Resources (NASA POWER) database through its public API.

Study Locations
Location	Latitude	Longitude	Climatic Zone
Colombo	6.9271	79.8612	Wet Zone
Badulla	6.9934	81.0550	Intermediate Zone
Jaffna	9.6615	80.0255	Dry Zone
API Configuration
Data Source: NASA POWER API
Parameter: UVI (Ultraviolet Index)
Temporal Resolution: Hourly
Community: RE (Renewable Energy)
Output Format: JSON
Study Period: January 2019 – December 2023
Example API Request
https://power.larc.nasa.gov/api/temporal/hourly/point?parameters=UVI&community=RE&longitude=79.8612&latitude=6.9271&start=20190101&end=20231231&format=JSON
Data Processing Workflow
Retrieve hourly UVI data from NASA POWER API.
Store downloaded data in JSON format.
Convert JSON records into tabular format (CSV).
Handle missing values using linear interpolation.
Perform lag selection using ACF and Mutual Information analysis.
Split data into training and testing sets.
Develop and evaluate ARIMA, RF, XGBoost, FNN, LSTM, CNN, and hybrid models.
Compare forecasting performance using MSE, RMSE, MAE, R², and Diebold-Mariano tests.
Reproducibility

All scripts used for:

Data acquisition
Data preprocessing
Feature engineering
Model training
Hyperparameter optimization
Model evaluation

are available in this repository.
