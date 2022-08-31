### SAPPHIRE model builder

This repository contains python code that allows the user to develop neural network classifiers for promoter prediction. The code can be modified and tailored to one's needs using the information below. 

#### Required input files: a genbank file, coordinates of transcription start sites (TSSs), coordinates of background sequences for training. Input should be formated like the examples found in the data folder.  

#### The architecture of choice can be specified in line 111. The CNN architecture was found to be the best performing one for promoter prediction in Pseudomonas and Salmonella. One of five provided architectures (code in architectures.py) can be chosen:
- fully connected neural network (build_fully_connected_NN)
- convoluational neural network (CNN) (build_CNN)
- recurrent neural network (RNN) (build_LSTM)
- CNN into RNN (build_CNN_LSTM)
- RNN into CNN into RNN (build_LSTM_CNN_LSTM) 





#### Class_weights for training are set to compensate for different amounts of TSS and background data for training. This can be modified in line 158

