Welcome to SPARTAN-Cloud's documentation!
===================================

**SPARTAN** (Surface PARTiculate mAtter Network) measures and provides surface ambient particulate matter (PM\ :sub:`2.5`\  and PM\ :sub:`10`\) concentration around the world, started in 2012. Currently, there are 29 active sites (as of Dec 2023). Check out `the SPARTAN website <https://www.spartan-network.org/>`_  for our collaborators worldwide!

SPARTAN sites are intentionally colocated with AERONET Sunphotometers to provide the only global dataset that directly connects ground-based PM2.5 and satellite remote sensing. In addition to filter-based PM\ :sub:`2.5`\  and PM\ :sub:`10`\  mass, SPARTAN also measures the chemical composition using IC, XRF, SSR, etc. Our SOPs can be found `here <https://www.spartan-network.org/standard-operating-procedures>`_. Measured chemical compostion together with total mass are reported in our :ref:`speciation product <speciation>`. We also reconstruct fine particulate matter into commonly studied chemical groups and repored with the :ref:`reconstructed fine mass product <RCFM>`. Aerosol scattering is also measured and :ref:`reported as our Nephelometer product <Neph>`. When both PM2.5 and fine aerosol scattering data are available, :ref:`time-resolved product <time-resolved>` at daily and hourly resolution are reported. More about our products on :ref:`SPARTAN data type <usage>`.

SPARTAN-on-cloud project provides fast and easy access to the latest SPARTAN data on
the `Amazon Web Services (AWS) cloud <https://aws.amazon.com>`_, supported by the `AWS Open Data Sponsorship Program <https://aws.amazon.com/opendata/open-data-sponsorship-program/>`_.

.. note::
   SPARTAN is a grass-roots network run by individual scientists who share their measurements as a public good. We request that you consult :ref:`our citation policy <citation-policy>` to credit developers when including SPARTAN data in your publications.

Contents
--------

.. toctree::

   api
   usage
   citation
