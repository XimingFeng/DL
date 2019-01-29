Batch Normalization
=======================

One of the assignment in class cs231n is to implement the function of bacth 
normalization, in both forward and backward propagation. Forward propagation is
pretty straigh forward but backward took me really long time to understand and 
implement. 

As you can see from the assignment, there are two ways to implement 
backpropagation.

* Simulate forward and backward prop through multiple steps
* Calculate the relationship between input and output. Then give a one step calculation.

No matter what method you want to choose, you have to draw a computation graph in order 
to help yourself to understand the operation dynamic. Below is the figure I had in my 
scratch paper. 




There some few things to note: 

* This figure did not show process from :math:`intmdt\_out` to :math:`out` in order to simplify the problem. 
* For the node that has two path coming out of it, the gradient should be the sum of the gradients calculated individually on different path. So in order to get the gradient of :math:`x_centered`, we need calculate the gradients with respect of path (1) and path (2) and add them together. 

-------------------
Simulation method
-------------------




