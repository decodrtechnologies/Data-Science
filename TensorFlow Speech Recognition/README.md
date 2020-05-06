# TensorFlow Speech Recognition Challenge

## Problem Statement:
Use the Speech Commands Dataset to build an algorithm that understands simple spoken commands. By improving the recognition accuracy of open-sourced voice interface tools, we can improve product effectiveness and their accessibility.


## DATA:
train.7z - Contains a few informational files and a folder of audio files. The audio folder contains subfolders with 1 second clips of voice commands, with the folder name being the label of the audio clip. There are more labels that should be predicted. The labels you will need to predict in Test are yes, no, up, down, left, right, on, off, stop, go. Everything else should be considered either unknown or silence. The folder _background_noise_ contains longer clips of "silence" that you can break up and use as training input.

The files contained in the training audio are not uniquely named across labels, but they are unique if you include the label folder. For example, 00f0204f_nohash_0.wav is found in 14 folders, but that file is a different speech command in each folder.

The files are named so the first element is the subject id of the person who gave the voice command, and the last element indicated repeated commands. Repeated commands are when the subject repeats the same word multiple times. Subject id is not provided for the test data, and you can assume that the majority of commands in the test data were from subjects not seen in train.

You can expect some inconsistencies in the properties of the training data (e.g., length of the audio).

test.7z - Contains an audio folder with 150,000+ files in the format clip_000044442.wav. The task is to predict the correct label. Not all of the files are evaluated for the leaderboard score.

- link to data: https://www.kaggle.com/c/tensorflow-speech-recognition-challenge/data

## Libraries used:
- Numpy
- Pandas
- Matplotlib
- Sklearn
- TensorFlow
- Keras

## Algorithm:
- Label Encoding
- CNN

## Steps involved:
1. Importing relevant python Libraries
2. Exploring the Dataset
3. Exploratory Data Analysis
4. Data Preprocessing
5. Model Building
6. Validation
7. Conclusion

## License:
 - Speech Commands Data Set v0.01
 - Creative Commons BY 4.0 license
 - Link : https://github.com/petewarden/extract_loudest_section
