# multi_hazard
This repository contains the data and code for analyzing landslide events using the COOLR dataset and ERA5 climate reanalysis data. The aim is to develop a predictive model using a Guzzy_LSTM approach to forecast the likelihood of landslide occurrences based on atmospheric conditions.
Data Description

The data folder includes Three datasets:

    COOLR Dataset: This dataset provides records of landslide events globally, detailing the date, location, and characteristics of each event.
    ERA5 Climate store: This consists of two datasets:
        Pressure Level Data: ERA5 atmospheric pressure levels for a 3x3 grid centered on the event's location.
        Precipitation Data: Precipitation measurements from ERA5 for the same 3x3 grid.

#Data Pre-processing

The data_preprocessing.ipynb file contains all the preprocessing steps applied to the COOLR dataset and ERA5 data, preparing them for analysis. Steps include:

    Data cleaning: Removing duplicates and handling missing values.
    Data transformation: Normalizing and standardizing pressure and precipitation data.


#Proposed Model

The fuzzy_lstm_model.ipynb file describes the development and training of the fuzzy_LSTM model, a hybrid approach that combines fuzzy logic with LSTM neural networks to enhance predictive accuracy. The model processes the pre-processed data to predict landslide risks based on environmental inputs.
Usage

To run the pre-processing scripts or model training:

    Ensure you have Python 3.8+ installed.
    Install required libraries using pip install -r requirements.txt.
    Execute Jupyter notebooks via jupyter notebook.
