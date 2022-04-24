# EMG-processing-CNN
This project aim to do EMG signal processing and then train it on CNN to predict flexion/extension.
This project has done many process on signal processing and machine learning. Overall process are these following step.
Hardware filter design >> signal aquisition >> signal processing >> data deviding >> CNN model train/test

Python coding only did on signal processing and CNN model training/testing

# signal processing 
  - signal processing will use raw data csv file names " EMG2.csv "
  - then open the python code file names " EMG processing "
  - then, you can run it all the cells
  - this processing compose of FFT to see amplitudes in frequency range to consider which frequncy need to be filtered out.
  - then, doing FIR low pass and high pass to clean signal and get the desired signal
  - Next, the signal value will be positive value using absolute function.
  - Finally, the signal will be filtered agian by FIR lowpass filter to simplify the signal shape.

# CNN model training/testing
  - this code will use the filtered signal from signal processing procedure
  - the data from filtered signal will be collect and devide in to 3 csv files named "train_set.csv","valid_set.csv" and "test_data.csv"
  - the class data files are also created in csv files named "class_tr.csv" and "calss_te.csv" 
  - then open the python code file names " CNN_EMG " 
  - then, you can run it all the cells
  - this process compose off data reshape to be compatible with CNN model
  - next, define CNN model architecture
  - next, train and validate CNN model
  - finally, test the model and find out accuracy
