# Gesture Recognition
> We build a CNN based model that can accurately recognize and interpret gestures performed by users in videos captured by a webcam. 
 


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
- We considered Conv3D-based models in the experiments.
- For 3D convolution, the base model was a COnv3D layer, followed by a deep layer and an output layer.
- Our final model turned out to be the simplest conceivable model: A conv3D layer and output layer.
- 89% training accuracy
- 87% validation accuracy
- 0.13 MB size
- 35337 parameters

## Conclusions
Our model is merely 0.13MB and can give about 89% and 87% accuracy on our training and validation data respectively. 

Such a light-weighing model would best suit our real-time application. Even our normalization process is fast since we just divide by 255 without spending time on computing mean and std dev. This makes our model extremely fast in runtime.

Since this is a real-time application of gesture recognition with quick movements, gesturing twice wouldn't be much of an inconvenience
and assuming an average accuracy of 88%, the probability of making an error twice would be just ~1.4%. 

This means that the probability of getting it rightly recognized in at most 2 attempts would be 98.6%, which is pretty high. 



**HENCE, OUR CURRENT MODEL IS PERFECTLY SUITABLE FOR THE ONLINE GESTURE RECOGNITION APPLICATION**

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
