.. DPPy documentation master file, created by
	 sphinx-quickstart on Tue Jun  5 07:45:55 2018.
	 You can adapt this file completely to your liking, but it should at least
	 contain the root `toctree` directive.

Welcome to DPPy's documentation!
################################

Determinantal point processes (DPPs) are specific probability distributions over clouds of points that have been popular as models or computational tools across physics, probability, statistics, and more recently of booming interest in machine learning. 
Sampling from DPPs is a nontrivial matter, and many approaches have been proposed. 
DPPy is a Python library that gathers all exact and approximate sampling algorithms for DPPs.

The purpose of this documentation is to both provide a quick survey of DPPs and relate each mathematical property with its implementation in DPPy. 
The documentation can thus be read in different ways:

	- if you read the sections in the order they appear, they will first take you through mathematical definitions and quick illustrations of how these definitions are encoded in DPPy. 
	- for more a traditional library documentation please refer to the corresponding API sections documenting the methods in each class, along with pointers to the mathematical definitions if needed. 
	- you can also directly jump to the Jupyter `notebooks <https://github.com/guilgautier/DPPy/tree/master/notebooks>`_, which showcase the use of some DPPy objects in more detail.

For another entry point to DPPy see the `companion paper <https://arxiv.org/abs/1809.07258>`_ :cite:`GaBaVa18`.

.. image:: _images/original_graph.png
   :width: 25%
.. image:: _images/kernel.png
   :width: 37.5%
.. image:: _images/sample_Wilson.png
   :width: 25%

As :ref:`exotic <exotic_dpps>` as it may sound the uniform measure on spanning trees of a graph is a DPP!

Installation instructions
=========================

See `README <https://github.com/guilgautier/DPPy/blob/master/README.md>`_

Documentation contents
======================

.. toctree::
  :maxdepth: 3

  finite_dpps/index
  continuous_dpps/index
  exotic_dpps/index
  bibliography/index
