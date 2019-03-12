YOLO
===================

See `Yolo Paper <https://arxiv.org/pdf/1506.02640.pdf>`_ 



################
Intro
################
Over all Sturcture/Pipeline:

1. Resize to 448 * 448
2. Conv Net
3. Threshhold the resulting detection by the model's confidence.  

A single conv net simultaneously predicts multiple bounding boxes and class probabilities for those boxes. It is trained on full image and directly optimizes detection performance. Benefit over traditional method of object detection.

1. Fast. Regression problem, no need for complex pipeline. High precision
2. Reason gloabally about the image when making prediction. 
3. Leans generalizable representation of objects. Less likely to break down when applied to new domain or unexpected inputs.

Drawback: 
Lag behind state-of-art detection system in accuracy. Struggle to precisely localize some objects. especially small ones 



########################
Resource 
########################

* `Yolo Paper <https://arxiv.org/pdf/1506.02640.pdf>`_ 
* `Project webpage <http://pjreddie.com/yolo/>`_
* `RCNN Paper <https://arxiv.org/pdf/1311.2524.pdf>`_