# FaceMaskDetection

## We open source all the popular deep learning frameworks' model and inference code to do face mask detection.
 + PyTorch
 + TensorFlow（include tflite and pb model）
 + Keras
 + MXNet
 + Caffe
 
 ** Detect faces and determine whether they are wearing mask.**

** First of all, we hope the people in the world defeat COVID-2019 as soon as possible. Stay strong, all the countries in the world.**

+ We make face mask detection models with five mainstream deep learning frameworks （PyTorch、TensorFlow、Keras、MXNet,Caffe） open sourced, and the corresponding inference codes.

![alt text](https://res.cloudinary.com/practicaldev/image/fetch/s--1u3Uz9sp--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/ojmek5e5tihf1p655ju6.png)

## MODEL STRUCTURE

We used the structure of SSD. However, in order to make it run quickly in the browser, the backbone network is lite. The total model only has 1.01M parametes.

Input size of the model is 260x260, the backbone network only has 8 conv layers. The total model has only 24 layers with the location and classification layers counted.

SSD anchor configurtion is show bellow:

|Multibox layers| feature map size| anchor size | aspect ratio|
|---------------|-----------------|--------------|-------------|
||First	         |33x33            |	0.04,0.056  |	1,0.62,0.42  |
