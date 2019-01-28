Part II: Modern Practical Deep Networks
========================================
Deep feedforward networks, also called feedforward neural networks, or multilayer perceptrons(MLPs). 

######################
Introduction
######################

* Goal: to approximate some function :math:`f^*(x)`. 
* Example: A classifier such as `Digit Recognizer <https://www.kaggle.com/c/digit-recognizer>`_ . We are trying to map an input :math:`\boldsymbol{x}` to a category :math:`y`. As the example of Digit Recognizer, the input is an image of hand written digit. We are trying to approximate this function :math:`f^*(x)` to map this image to the correct digit. 

It forms the basic of many important commercial application such as Convolutional Neural Network and Recurrent Neural Network. 

##############################################
Why we call it Network?
##############################################

It represent the combination of different functions. For example, we might have three functions :math:`f_1, f_2 and f_3` connectedin a chain, to form :math:`f(x) = f_3(f_2(f_1(x)))`. These chain structures are the most commonly used structures of neural networks. In this case, :math:`f_1` is called the ﬁrst layerof the network, :math:`f_2` is called the second layer, and so on. 

The ﬁnal layer of a feedforward network is called theoutput layer. During neural network training, we drive :math:`f(x)` to match :math:`f^∗(x)`.

###############################################
Hidden Layers
###############################################
The training examples specify directly what the output layer must do at each point :math:`x`; it must produce a value that is close to :math:`y`. The behavior of the other layers is not directly speciﬁed by the training data. The learning algorithm must decide how to use those layers to produce the desired output, but the training data do not say what each individual layer should do. Instead, the learning algorithm must decide how to use these layers to best implement an approximation of :math:`f^∗`. Because the training data does not show the desired output for each of these layers, they are called hidden layers

##################
Chapters
##################
.. toctree::
   :maxdepth: 2

   Optimization for Training Deep Models/index
