Greek Sign Language Recognition project
---------------------------------------

This folder contains the model preparation scripts.
Below is the runtime order:

- 1_unique_words.py: reads the initial dataset csv and extracts all the unique words.
                     Then a new csv is created containing the paths for the videos for each unique word.

- 2_create_dataset.py: reads the csv generated above and creates a new csv containing every example with each annotated class.

- 3_undersampling.py: makes an undersampled dataset to exactly 500 examples

- 4_holistic_static.py: for each row in the csv generated by 2 (or 3), use Mediapipe to generate a csv containing
                        the selected body points for each video file. The columns of the csv contain the flattened body points of a frame
                        (x,y), while the rows denote the frames (video sequence).

- 5_model_pytorch.py: training and evaluation of the model using the dataset from 4.

- 6_test_model.py: testing the saved model from 5.

- 7_live_test.py: live demonstartion of LSTM model prediction (needs webcam!)

- annotate_img.py: generates the selected upper body points and saves them in blank images.