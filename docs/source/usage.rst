SPARTAN data types
=====

.. _Overview:

Overview
------------

SPARTAN provides open access, pre-generated data sets from all of our sites, started in 2012. Currently, there are 29 active sites (as of Dec 2023). 

SPARTAN sites are intentionally colocated with AERONET Sunphotometers to provide the only global dataset that directly connects ground-based PM2.5 and satellite remote sensing. In addition to filter-based PM\ :sub:`2.5`\  and PM\ :sub:`10`\  mass, SPARTAN also measures the chemical composition using IC, XRF, SSR, etc. Our SOPs can be found `here <https://www.spartan-network.org/standard-operating-procedures>`_. Measured chemical compostion together with total mass are reported in our :ref:`speciation product <speciation>`. We also reconstruct fine particulate matter into commonly studied chemical groups and repored with the :ref:`reconstructed fine mass product <RCFM>`. Aerosol scattering is also measured and :ref:`reported as our Nephelometer product <Neph>`. When both PM2.5 and fine aerosol scattering data are available, :ref:`time-resolved product <time-resolved>` at daily and hourly resolution are reported. All products are presented as csv files and reported by site. 

SPARTAN is a grass-roots network run by individual scientists who share their measurements as a public good. We request that you consult :ref:`our citation policy <citation-policy>` to credit developers when including SPARTAN data in your publications.

.. _Speciation:
PM2.5 & PM10 speciation
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

.. _RCFM:
Reconstructed Fine Mass
----------------

.. _Neph:
Nephelometer data
----------------


.. _time-resolved:
Time resolved PM2.5 
----------------


