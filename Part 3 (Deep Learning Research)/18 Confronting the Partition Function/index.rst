18 Confronting the Partition Function
=======================================

Review:

An undirected graphical model is a structured probabilitic model defined on an undirected graph G. For each clique C in the graph, a factor :math:`\phi(C)` (also called a clique protential) measures the affinity of the variables in that clique for being in each of their possible joint states. :math:`\phi(C) > 0`. Unnormalized probability distribution:

.. math::
	\hat{p}(x) = \prod_{C\in G}\phi(C)

**A clique of the graph is a subset of nodes that are all connected to each other by an edge of the graph.**

**To obtain a valid probability distribution, we must use the corresponding normalized probability distribution.**

.. math::
	
	p(x) = \frac{1}{Z}\hat{p}(x)

**where Z is the value that results in the probability distribution summing or integrting to 1**

.. math::
	
	Z = \int \hat{p}(x)dx

You can think of Z as constant when :math:`\phi` functions are held constant. Note that if the :math:`\phi` functions have parameters, then Z is a function of those parameters. Normalizing function Z is known as partition function.

Computing Z is intractable for many interesting models. How to confront the challenge

* models designed to have a tractable normalizing constant
* designed to be used in ways that do not involve comupting p(x) at all.
* directly confront the challenge of intractable partition function, as described in this chapter

.. toctree::
   :maxdepth: 1

   18.1 The log-likehood Gradient
   18.2 Stochastic Maximum Likehood and Contrastive
   18.3 Pseudolikehood
   18.4 Score Matching and Ratio Matching
   18.5 Denoising Score Matching
   18.6 Noise-Contrastive Estimation
   18.7 Estimating the Partition Function
