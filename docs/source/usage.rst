SPARTAN data types
=====

.. _Overview:

Overview
------------

SPARTAN provides open access, pre-generated data sets from all of our sites, started in 2012. Currently, there are 29 active sites (as of Dec 2023). 

SPARTAN sites are intentionally colocated with AERONET Sunphotometers to provide the only global dataset that directly connects ground-based PM2.5 and satellite remote sensing. In addition to filter-based PM\ :sub:`2.5`\  and PM\ :sub:`10`\  mass, SPARTAN also measures the chemical composition using IC, XRF, SSR, etc. Our SOPs can be found `here <https://www.spartan-network.org/standard-operating-procedures>`_. Measured chemical compostion together with total mass are reported in our :ref: `speciation product <speciation>`. We also reconstruct fine particulate matter into commonly studied chemical groups and repored with the :ref: `reconstructed fine mass product <RCFM>`. Aerosol scattering is also measured and :ref: `reported as our Nephelometer product <Neph>`. When both PM2.5 and fine aerosol scattering data are available, :ref: `time-resolved product <time-resolved>` at daily and hourly resolution are reported. All products are presented as csv files and reported by site. 

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


.. _citation-policy:
SPARTAN data citation policy
----------------
Each site has Principal Investigator(s) (PI) who is responsible for instrument operation. PI contact information can be found on the `SPARTAN website <https://www.spartan-network.org/data>`_. We encourage you to contact the site PI when data for a particular site are used. Data from all sites are analyzed at Washington University in St. Louis for mass and composition. We also encourage you to contact Chris Oxford and Randall Martin at SPARTAN.PM25@gmail.com when SPARTAN data are used.

We recommend the following citations for use of SPARTAN data for referencing our sampling methods and data analysis techniques:
   SPARTAN: a global network to evaluate and enhance satellite-based estimates of ground-level particulate matter for global health applications Snider, G. et al. : Atmos. Meas. Tech., 8, 505-521, 2015 , doi:10.5194/amt-8-505-2015.
   ​
   Variation in Global Chemical Composition of PM2.5: Emerging Results from SPARTAN Snider, G., et al.: Atmos. Chem. Phys. 16, 9629-9653, 2016 doi:10.5194/acp-16-9629-2016.
​​​   
   Large global variation in measured airborne metal concentrations driven by anthropogenic sources McNeill, J. et al. : Sci. Rep., 10, 21817, 2020 doi: https://doi.org/10.1038/s41598-020-78789-y

When publishing data from a few sites, please consider authorship for the site PI(s) and the following acknowledgement:
   We thank the SPARTAN project for its effort in establishing and maintaining (site name(s)) sites. 

Please send a copy of the paper to Chris Oxford, Xuan Liu and Randall Martin at SPARTAN.PM25@gmail.com for a quick review prior to submission. Upon final publication, please send a copy of the paper to Chris Oxford at our SPARTAN email address, SPARTAN.PM25@gmail.com for posting on the SPARTAN website.

When publishing data from many sites:
If SPARTAN data are the main component of the paper than we encourage offering co-authorship to the following investigators: Chris Oxford, Xuan Liu, Yinon Rudich, Michael Brauer, and Randall V. Martin.
​
