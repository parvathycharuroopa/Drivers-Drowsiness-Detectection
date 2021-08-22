# Drivers-Drowsiness-Detectection
A model to Detect Drivers Drowsiness using Transfer Learning

dataset used : MRL eye Dataset
In the dataset, we annotated the following properties (the properties are indicated in the following order):
subject ID; in the dataset, we collected the data of 37 different persons (33 men and 4 women)
image ID; the dataset consists of 84,898 images
gender [0 - man, 1 - woman]; the dataset contains the information about gender for each image (man, woman)
glasses [0 - no, 1 - yes]; the information if the eye image contains glasses is also provided for each image (with and without the glasses)
eye state [0 - closed, 1 - open]; this property contains the information about two eye states (open, close)
reflections [0 - none, 1 - small, 2 - big]; we annotated three reflection states based on the size of reflections (none, small, and big reflections)
lighting conditions [0 - bad, 1 - good]; each image has two states (bad, good) based on the amount of light during capturing the videos
sensor ID [01 - RealSense, 02 - IDS, 03 - Aptina]; at this moment, the dataset contains the images captured by three different sensors
(Intel RealSense RS 300 sensor with 640 x 480 resolution, IDS Imaging sensor with 1280 x 1024 resolution, and Aptina sensor with 752 x 480 resolution)

**Working**
The input is video (real time web cam) from the video face/eyes are detected and these images are fed to a deep learning model which checks if the 
eyes are opened or closed. a timer would run and if the eyes are shut for continuous 5 seconds, the system would generate an alarm saying that the person is drowsy
