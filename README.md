# ML_corn_yield_analysis
Data from NASS and NOAA were compiled to forecast corn yield. 

Here we see three different models: Single hidden layer NN, Neural Network with 3 hidden layers using the functional API and transformer archecture model using rain and temperature data from January to July.

Goal - Minimum RMSE (bu/acre) with a generalization ratio (MAE) of < 1.25

Results:
  Keras Sequential:\n 
    Features: Genetic Data
    RMSE Train: 29.67
    RMSE Validaton: 29.80 
    RMSE Test: 31.89
    Generalization Train/Validation MAE: 1.05

  Keras Functional API FFNN:
    Features: Genetic Data, Location (Ag District, State-County)
    RMSE Train: 20.84 bu/acre
    RMSE Validaton: 21.12 bu/acre
    RMSE Test: 20.96 bu/acre
    Generalization Train/Validation MAE: 1.08

 Keras Transformer Model:
    Features: Rain and Temp (Jan - July), Genetic Data, State-Country
    RMSE Train: 15.14 bu/acre
    RMSE Validaton: 17.77 bu/acre
    RMSE Test: 16.60 bu/acre
    Generalization Train/Validation MAE: 1.18

NOTE: This is work completed in introduction to ML. All the models presented above were created by me.



    
  
