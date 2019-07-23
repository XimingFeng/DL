19 Approximate Inference
============================

* v: visible variables
* h: hidden variables

Challenge of inference: compute p(h|v) or take expectation with respect to it.


Review:

.. image:: rsc/Figure16.6.PNG

.. image:: rsc/Figure16.7.PNG

.. image:: rsc/Figure16.8.PNG


Direct interaction in undirected model / explaining away interaction between mutual ancestors of the same visible unit in directed model ==> interaction between latent variables => Intractable inference problem.

.. image:: rsc/Figure19.1.PNG


.. toctree::
   :maxdepth: 1

   19.1 Inference as Optimization
   19.2 Expectation Maximization
   19.3 MAP Inference and Sparse Coding
   19.4 Variational Inference and Learning 
   19.5 Learned Approximate Inference
   

   