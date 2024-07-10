SPARTAN data types
=====

.. _commonality:
Commonality
------------
All products are presented as CSV files and reported by sites. At the beginning of each file, there is a data version and date of update. Basic site information (name, location, etc) is provided at the first few columns of the file, followed by the dates of the samples. Because some samples applied the `9-day sampling method <>`, some files give the start and end dates of the sample. The reported variables can be identified by either Parameter_Name or Parameter_Code. The last few columns provide information on the methodology and quality check. A comprehensive list of the methodologies is `here <>`. 

The following sections give brief introductions and examples of each data type. 

Additional information on the sites can be found on the `Site Info Sheet <>`.


.. _Speciation:
PM2.5 & PM10 speciation
----------------
The PM2.5 & PM10 speciation product report the direct measurements of total mass and chemical composition including water soluble ions from IC, trace elements from XRF and ICPMS, carbons from SSR, HIPS, and FTIR. Relevant SOPs are reported on the `official SPARTAN website <https://www.spartan-network.org/standard-operating-procedures>`_. 

.. literalinclude:: FilterBased_ChemSpecPM25_AEAZ_example.csv
   :language: text

.. _RCFM:
Reconstructed Fine Mass
----------------
The reconstructed fine mass builds on the speciation data to provide estimation of ammoniated sulfate, ammonium nitrate, sea salt, fine soil (dust), equivalent BC/EC, trace element oxides, and residual matters (assumed to be organics). Based on the estimated composition, the k-Kohler constant can also be estiamted. More can be found in the `SOP <https://www.spartan-network.org/_files/ugd/6321a4_55403d40877b4be7a06064fe1244d891.pdf>`_. 

.. literalinclude:: FilterBased_ReconstrPM25_AEAZ_example.csv
   :language: text

.. _Neph:
Nephelometer data
----------------
Nephelometer scatter data provide high temporal resolution information and particle size information, offering unique insights for satellite remote sensing. Details on the operation is reported `here <https://www.spartan-network.org/_files/ugd/6321a4_d2614db581494ba0a10d17ccbc9f8a6c.pdf>`_. 

.. literalinclude:: NephelProcd_HourlyScaPM10_AEAZ_example.csv
   :language: text


.. _time-resolved:
Time resolved PM2.5 
----------------
We constrain the Nephelometer data with filter based mass concentration to yield the daily and hourly resolved products. The procudure is reported `here <https://www.spartan-network.org/_files/ugd/6321a4_7437804cc21c40d9aff1502ff342b4a5.pdf>`.
.. literalinclude:: TimeResPM25_HourlyEstPM25_AEAZ_example.csv
   :language: text


