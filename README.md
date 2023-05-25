# Drone_Noise
## Drone Health Monitoring using audio classification of propeller sound 
## Approach:
#### 1. Expansion of available dataset using GANs as the number of blades, length of blades, propeller speed, noise in the surroundings etc. all vary from situation to situation and we have a limited dataset
#### 2. Preprocessing to obtain spectrograms and MFCC co-efficents 
#### 3. Training of various models like CNNs, LSTMs, and Transformer Encoder and Classification of propeller audio into 4 categories- All propellers working, 1 propeller broken, 2 propellers broken, 3 or more propellers broken, looking into whether it is possible to output the configuration/position of the damaged propellers 
#### 4. Evaluation of metrics like F1 score, precision, recall, and computational power requirement
#### 5. Filtering out surrounding noise when the microphone records propeller audio
#### 6. Deployment of the trained model on a microcontroller like Arduino using TinyML frameworks like TensorFlow Lite
