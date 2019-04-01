YOLO 2
==================

##########################
1. Introduction
##########################

Comparison:

* Object Detection: less dataset, less labels/tags/class
* Classification Problem: more dataset, more labels/tags/class

Our method uses a herachical view of object classification that allows us to combine distinct datasets together.

A joint training algorithm that allow to train detectors on both detection and classification data. The model leverages labeled detection images to learn to precisely localize objects while it uses classification images to increase its vocabulary and robustness. 

This model 

1. Improve the base detector YOLO to YOLOv2.
2. use dataset combination method and joint training algorithm to train model 

##########################
2. Better
##########################

Shortcomings compared to region proposal-based method:

1. Significant number of localization errors..
2. Low recall 

Thus YOLO2 focus mainly on improving recall and localization while maintaining classification accuracy.

Computer Vision generally trends towards larger and deeper networks. intead of scaling up the network, YOLO2 simplify the network and then make the representation easier to learn. Ideas to achieve this

* Batch Normalization: with batch normalization, we can remove dropout from the model without overfitting (more than 2% mAP increase).
* High Resolution Classification (4% mAP increase): 

	* First fine tune the classification network at the full 448 * 448 resolution for 10 epochs on ImageNet. -> Gives the network time to adjust its filter to work better on higher resolution input. 
	* Then fine tune the resulting network on detection. 

* Convolution With Anchor Boxes
