# Neural_Network_Charity_Analysis
## Overview
The purpose of this analysis was to train a neural network model to predict whether money donated to an organization would be used successfully and for its intended purpose.
## Results
### Data Processing
#### Target Variable
 - IS_SUCCESSFULL
#### Feature Variables
- APPLICATION_TYPE
- AFFILIATION      
- CLASSIFICATION         
- USE_CASE                  
- ORGANIZATION                 
- STATUS                      
- INCOME_AMT                  
- SPECIAL_CONSIDERATIONS
- ASK_AMT
#### Variables Removed
- EIN
- NAME

These variables were removed due to them simply being identification information.
### The Model
- Neurons: 23
- Layers: 4
- TanH was selected for the first two hidden layers
- ReLU was selected for the last two hidden layers
- Sigmoid was selected for the output layer

Originally there were 13 neurons and 2 layers but more were added in an attempt to improve the performance of the model. The activation functions were selected becuase they were the best performing for each layer. Unfortunetly I was unable to achieve the target model performance of 75%. In an attempt to improve the model performance I added extra neurons/layers, attempted different activation functions, and tried binning data in the ASK_AMT column.
## Summary
Overall the accuracy of the deep learning model was okay. I would recommend trying to use a random forest model to see if less moving parts in the code lead to an easier time optimizing the model.
