<<<<<<< HEAD
Traffic Sign Detection Based on Faster R-CNN
by Jiaxi Nie, Rui Lan, Yuan Cheng 

This project is forked from https://github.com/yhenon/keras-frcnn

Autonomous driving technology has been a key aspect of artificial intelligence throughout the past three decades and has successfully commercialized recently. Object detection has been on the center of the stage as a critical part of autonomous driving and other traffic-related applications. People have striven to detect and analyze road conditions to ensure safe and effective driving, focusing on recognizing pedestrians, automobiles, roads and traffic signs, etc. Our project focuses on detecting traffic signs from provided images by using deep learning techniques. We perform Faster Region Based Convolutional Neural Network (Faster R-CNN) to localize and recognize different traffic signs on The German Traffic Sign Detection Benchmark (GTSDB) dataset. We show our Faster R-CNN is useful in detecting the traffic signs accurately and efficiently. 

# keras-frcnn
Keras implementation of Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks.

pretrained vgg-16 model can be downloaded from: https://gist.github.com/nitish11/73ba862753929e08b3b319ff1e8c9c09
To run:
run script file: run.sh

Parameters to change:
- anchor size
- anchor ratio
- RPN stride
- CNN model

This program contains two parts: 
1)In training process, it takes batches of training images with ground truth boxes and labels as input, trains the model by several epochs, then saves the trained model as .h5 file. 
2)In testing process, it takes batches of testing images and the trained model as input, generates the predicted boxes with class label and confident score, saves the results as .png file.  
=======
# Traffic Sign Detection
Traffic sign detection based on Faster R-CNN, implemented in Keras. The annotated dataset comes from German Traffic Sign Detection Benchmark.

Notes:
- config.py contains all settings for the train or test run. The anchor box sizes are selected from [8, 16, 32, 64] and anchor ratios from [1:1, 1:2, 2:1].
- The base network shared by RPN and classifier are implemented in 2-layer FCnet, ZFnet and VGG16.
- The RPN Stride depends on network structure and should be modified correspondingly if a new model/structure is employed.

Example output:

![ex1](https://imgur.com/vkH58TY.png)
![ex2](https://imgur.com/y1cYou4.png)
>>>>>>> 982362edde9ea5a11dd5039c25bf5dee3670978f


