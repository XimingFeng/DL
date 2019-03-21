15 Representation Learning 
============================

Information processing could be easy or difficult depending on how the information is represented.

Eg 1:

* 210 / 6: easy, straightforward.
* CCX / VI: difficult.

Eg2 Insert a number into

* sorted linked list: O(n) runtime
* red-black tree: O(log n) 

Feedforward network trained by supervised learning: last layer linear classifier or nearest neighbor classifier. The rest of the network learns to provide a representation to this classifier. Training with a supervised criterion naturally leads to the representatino at every hidden layer taking on properties that make the classification easier.

Just like superviser network, unsupervised deep learning algorithms have a main training objective but also learn a representation as a side effect. Most of representation learning problem face the trade off between

* Researve as much info about input as possible
* attain nice properties such as independence



.. toctree::
	:maxdepth: 1
	:caption: Contents:

	15.1 Gready Layer Wise Unsupervised Pretraining
	15.2 Transfer Learning and Domain Adaptation
	15.3 Semi Supervised Disentangling of Casual Factors 
	15.4 Distributed Representation
	15.5 Exponential Gains from Depth
	15.6 Providing Clues to Discover Underlying Causes
