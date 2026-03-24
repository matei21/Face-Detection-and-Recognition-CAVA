**Facial Detection and Face Recognition project for Scooby Doo dataset**

The project files are:
-**antrenare**: folder containing the data for training, images of the characters from the Scooby-Doo cartoon.
-**evaluare**: folder structure:
  -cod_evaluare: code written for the evaluation of the models, generating the mAP curve
  -fake_test: images for testing
  -fisiere_solutie: 333_MateiOctavianAndrei: 
    -task1_cnn: Jupyter Notebook with the code for solving Task 1 of the project, meaning the implementation of our own model in order to detect faces in an image.
    -task1_yolo: Jupyter Notebook with the code for solving Task 1 of the project using a YOLO or any SOTA model that surpasses 90% accuracy in order to test it against our own model.
    -task2_cnn: Jupyter Notebook with the code for solving Task 2 of the project, meaning the implementation of our own model in order to detect the characters in an image.
    -task2_yolo: Jupyter Notebook with the code for solving Task 2 of the project using a YOLO or any SOTA model that surpasses 90% accuracy in order to test it against our own model.
-validare: validation images

The Project Report can be viewed here:
https://github.com/matei21/Face-Detection-and-Recognition-CAVA/blob/main/Project%20Report%2C%20Matei-Octavian%20Andrei%20333%20(1).pdf

The architecture of the models:
-Hard Negatives Mining: mining parts of images that the model usually detects as fake positives, in order for it to learn to avoid labeling those ones as positive.
-NMS: non-maximal suppresion - when we have 2 or more detections that overlap each other too much (the Intersection-Over-Union is higher than a certain threshold set by the developer), the best one is selected and the rest of them are discarded.
-PyTorch architecture for the Convolutional Neural Network, using DirectML or CUDA to speed up the training. 
