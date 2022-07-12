### Data Collection:


### Data Processing
- Convert Year-Month-Day-Hour individual columns to single datetime columns
- MinMax Scaling
- 7:3 Train-Test Ratio

### Stacked LSTM Model

Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
lstm (LSTM)                  (None, 7, 32)             4352      
_________________________________________________________________
lstm_1 (LSTM)                (None, 7, 64)             24832     
_________________________________________________________________
lstm_2 (LSTM)                (None, 7, 128)            98816     
_________________________________________________________________
lstm_3 (LSTM)                (None, 256)               394240    
_________________________________________________________________
dropout (Dropout)            (None, 256)               0         
_________________________________________________________________
dense (Dense)                (None, 1)                 257       
=================================================================
Total params: 522,497
Trainable params: 522,497
Non-trainable params: 0
_________________________________________________________________

### Predictions:

RMSE (CTG):
RMSE (KHU):
RMSE (SYL):
RMSE (RAJ):
