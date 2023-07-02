# Gesture Recognition
> We build a CNN/RNN based model that can accurately recognize and interpret gestures performed by users in videos captured by a webcam. 
 


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Results](#results)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- The problem at hand involves developing a feature for smart televisions that can recognize and interpret 
different gestures performed by users.
- These gestures are monitored by the TV's built-in webcam and correspond to specific commands. 
- In this project, we use CNN/RNN based model that can accurately recognize and interpret 5 gestures performed by users in videos captured by a webcam.
- The training and validation data is formed from the [Kaggle](https://www.kaggle.com/datasets/imsparsh/gesture-recognition).
- We build upon one CNN/RNN based model architecture.
- The 5 gestures are given below

Gesture | Interpretation
--- | ---
Thumbs up | Increase volume
Thumbs down | Decrease volume
Left swipe | 'Jump' backward 10 seconds
Right swipe | 'Jump' forward 10 seconds
Stop | Pause the movie
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Results
- Both Conv3D and RNN-based models were considered in the experiments.
- For 3D convolution, the base model was a single Conv3D layer model.
- For RNN, a basic model with 1 Conv2D, 1 GRU, and 1 Dense layer was employed.
- Using the Conv3D-based model, we were able to best achieve 74% validation accuracy.
-  Using LSTM based model, we were able to best achieve 71% validation accuracy
-  Both are decent results. But let's compare the total number of parameters:
    - Conv3D-based model: 17,393,797
    - LSTM-based model: 1,186,885

## Conclusions
- With just 7% of the parameters used by the Conv3D-based model, our LSTM-based model brings about the same accuracy (71% validation accuracy).
- Thus, the LSTM-based model would be our final model

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Keras - version 2.12.0
- Tensorflow - version 2.12.0
- Pillow - version 8.4.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->



## Contact
Created by [@showman-sharma] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
