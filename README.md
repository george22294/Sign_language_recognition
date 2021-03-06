# Sign_language_recognition
This project is about Sign language recognition using Mediapipe framework applied in video frames.

Sign language recognition problem requires a plethora of computational and equipment resources for a required feature representation to express every hand gesture. Various studies have proposed different deep learning and machine learning approaches using depth images to achieve extremely high accuracy. In this work, we propose a solution based on the [Mediapipe](https://google.github.io/mediapipe/) framework for extracting the body points from video frames, and on Neural Networks and the SVM classifier that accept them as input. The outcomes proved to be satisfactory given the chosen preprocessing methods that yielded 94-95% F1 macro score on the test set for 10 glosses as classes. 

## Code

In directory _code_ you can find the corresponding directories which refer to the pythons scripts which were tested on Ubuntu or Windows 10, respectively. Each one of these cointains the appropriate README.txt file where you can find the details on how to run them. In addition, in README files you can figure out where to find the dataset used, the structure to be given in your own dataset if you want to use another one, and how to use it.

## Dataset

The dataset used for the implementation and testing of deep learning models as well as SVM is _GSL_ which can be found [here](https://vcl.iti.gr/dataset/gsl/).
It is important to be mentioned that only the isolated samples of this dataset were used.

For more insights, you could read the report.

The above demos is in slow motion so that the outocomes are easily perceived. After 10 frames, predictions are produced using the model which corresponds to _Archtecture 1_ described in report. Note that the predictions are different for consecutive frames, meaning that the predictions apply in sliding windows with window size to be equal to 10.

<img src="https://github.com/george22294/Sign_language_recognition/blob/main/demos/first_demo.gif"/>

<img src="https://github.com/george22294/Sign_language_recognition/blob/main/demos/second_demo.gif"/>



