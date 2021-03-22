comp-syn
~~~~~~~~

comp-syn is a python package which provides a novel methodology to explore relationships between abstract concepts and color. We provide functionalities to create a dataset for word - image associations through Google Cloud and WordNet, as and demonstrate a variety of image and word related analyses. We introduce constructs such as *Colorgrams* as a tool for analysis, as well as the ability to create *color representational vectors* for images, and words as aggregations of images. Our work demonstrates a strong relationship between abstract semantic domains and colors, and supports claims for collective cognition and embodied cognition. The package allows you to explore these relationships yourself!

The theoretical frameword is described in:

Douglas Guilbeault , Ethan Nadler, Mark Chu, Ruggiero Lo Sardo, Aabir Abubaker Kar, and Bhargav Srinivasa Desikan. "Color Associations in Abstract Semantic Domains." *Forthcoming in Cognition* (2020).

The work arose through a collaboration between the contributors at the Santa Fe Institute's Complex System Summer School 2019. 


Documentation and Examples
~~~~~~~~~~~~~~~~~~~~~~~~~~

The
`notebooks <https://github.com/comp-syn/comp-syn/tree/master/notebooks>`__
directory showcases the usage of compsyn, with examples and basic usage.

We currently provide functionality to download and organise image data to be loaded as vector objects, as well as a preliminary analysis using them.


Installation
~~~~~~~~~~~~

Run ``pip install compsyn`` to download and install from PyPI.

Run ``python setup.py install`` for default installation.

Run ``pip install .`` to install from source.


Dependencies
~~~~~~~~~~~~

-  Python 2.7+, 3.4+
-  numpy, scipy, scikit-learn, matplotlib, PIL

Notes
~~~~~

To use the package one would need to download the JzAzBz array to convert the images to the appropriate vector form. It can be downloaded here (`link <https://drive.google.com/file/d/1wspjIBzzvO-ZQbiQs3jgN4UETMxTVD2c/view>`_). We provide sample images downloaded from Google Images to test the functionality.


Compsyn V1.0.0
~~~~~~~~~~~~~~

- New image analysis techniques (wavelet with PCA)
- Introduces the Trial dataclass for creating logically separated datasets
- Optional shared backend via S3, trials can be saved with specific "revision" names, data easily shared
- Re-worked notebooks as documentation of the API to Vectors


Shared Backend with S3
~~~~~~~~~~~~~~~~~~~~~~

- raw data and Vector objects can be saved remotely for collaboration
- saving vectors or data to the backend is done by creating a "revision"
