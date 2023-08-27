# Drone_Noise
## Drone Health Monitoring using audio classification of propeller sound 
## Approach:
#### 1. Expansion of available dataset to generalise to various propellers as the number of blades, length of blades, propeller speed, noise in the surroundings etc. all vary from situation to situation and we have a limited dataset
#### 2. Preprocessing to obtain spectrograms and MFCC co-efficents 
#### 3. Training of various models like CNNs, LSTMs, and Transformer Encoder and Classification of propeller audio into 4 categories- All propellers working, 1 propeller broken, 2 propellers broken, 3 or more propellers broken, looking into whether it is possible to output the configuration/position of the damaged propellers 
#### 4. Evaluation of metrics like F1 score, precision, recall, and computational power requirement
#### 5. Filtering out surrounding noise when the microphone records propeller audio
#### 6. Deployment of the trained model on a microcontroller like Arduino using TinyML frameworks like TensorFlow Lite

### References:
#### 1. REAL-WORLD ON-BOARD UAV AUDIO DATA SET FOR PROPELLER ANOMALIES Sai Srinadhu Katta , Kide Vuojarvi , Sivaprasad Nandyala, Ulla-Maria Kovalainen, Lauren Baddeley : https://github.com/tiiuae/UAV-Propeller-Anomaly-Audio-Dataset/blob/main/REAL-WORLD%20ON-BOARD%20UAV%20AUDIO%20DATA%20SET%20FOR%20PROPELLER%20ANOMALIES.pdf - Trained CNNs, LSTMs, Transformer Encoders on the audio dataset they obtained during the entire flight time 
#### 2. An Audio-Based Fault Diagnosis Method for Quadrotors Using Convolutional Neural Network and Transfer Learning: https://arxiv.org/pdf/2003.02649.pdf - Spectrogram analysis using CNNs, then using transfer learning to use features learnt on one quadcopter to train the model for another with minimal training data
#### 3. Audio-Based Drone Detection and Identification Using Deep Learning Techniques with Dataset Enhancement through Generative Adversarial Networks- https://www.mdpi.com/1424-8220/21/15/4953 - Dataset enhancement using GANs, CNN, RNN, and R-CNN based models were used 
#### 4. Experimental analysis on the noise of propellers for small UAV - https://www.sciencedirect.com/science/article/abs/pii/S0003682X12001715
#### 5. An Audio-Based Fault Diagnosis Method for Quadrotors Using Convolutional Neural Network and Transfer Learning - Wansong Liu, Zhu Chen, Minghui Zheng - https://arxiv.org/pdf/2003.02649.pdf
#### 6. An Intelligent Fault Diagnosis Approach for Multirotor UAVs Based on Deep Neural Network of Multi-Resolution Transform Features - https://www.mdpi.com/2504-446X/7/2/82
#### 7. A guide for using the Wavelet Transform in Machine Learning- https://ataspinar.com/2018/12/21/a-guide-for-using-the-wavelet-transform-in-machine-learning/
