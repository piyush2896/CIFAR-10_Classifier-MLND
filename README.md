# CIFAR-10 Classifier MLND Project
This is my project for Deep Learning Module of Machine Learning Engineer Nanodegree by Udacity. 
The model is written using core functionalities of TensorFlow

## Model Description

| Layer Number 	| Layer Type     	| Description             	|
|--------------	|----------------	|--------------------------	|
| 1            	| conv2d_maxpool 	|3x3, 64,  1x1, 2x2, 2x2*   |
| 2            	| conv2d_maxpool 	|3x3, 128, 2x2, 2x2, 2x2*   |
| 3            	| conv2d_maxpool 	|3x3, 256, 2x2, 2x2, 2x2*   |
| 4            	|     flatten    	|out=256                   	|
| 5            	|     dropout    	|keep_prob=0.5     	       	|
| 6            	|   dense_layer  	|out=2048, ReLu            	|
| 7            	|     dropout    	|keep_prob=0.5     	       	|
| 8            	|   dense_layer  	|out=1024, ReLu            	|
| 9            	|   dense_layer  	|out=512, ReLu             	|
| 10           	| output (Logit) 	|out=10, Linear            	|

* Convolution Ksize, No. of Kernels, Convolution strides, Max Pool Ksize, Max Pool strides

## Final Results
Test Accuracy: 0.6976

## A Sample From Test
![](result.png)