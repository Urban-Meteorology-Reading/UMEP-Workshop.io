.. _Consider1:

Model Inputs
------------

- `Files required to run SUEWS <https://suews.readthedocs.io/en/latest/input_files/input_files.html>`_
- The data are needed for every grid (can be any shape) area in the domain to be modelled.

Model Physics options
=====================

- `RunControl <https://suews.readthedocs.io/en/latest/input_files/RunControl/RunControl.html>`_

- the selection of which submodels are to be used
- choose after the other decisions
 


Forcing data
============

- `Meteorological variables needed <https://suews.readthedocs.io/en/latest/input_files/met_input.html>`_

Data Sources
~~~~~~~~~~~~~

- Observations
- Climate data e.g. ERA5, projections
- Coupled Model e.g. WRF

Height consideration of the forcing data
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- `Several heights need to be considered <Height>`


Site Information
================


- `Site parameters <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_SiteInfo.html>`_

 .. list-table:: Site parameters
   :header-rows: 1
   :widths: 30, 30, 30, 30

   * - Function  :ref:`T1-f`
     - Materials :ref:`T1-m`
     - Biophysical :ref:`T1-gs`
     - Water :ref:`T1-w`
  * - `SUEWS_AnthropogenicEmission <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_AnthropogenicEmission.html>`_
     - `SUEWS_NonVeg <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_NonVeg.html>`_
     - `SUEWS_BiogenCO2 <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_BiogenCO2.html>`_
     - `SUEWS_Irrigation <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Irrigation.html>`_
   * - `SUEWS_Irrigation <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Irrigation.html>`_ 
     - `SUEWS_OHMCoefficients <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_OHMCoefficients.html>`_
     - `SUEWS_Conductance <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Conductance.html>`_
     - `SUEWS_Profiles <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Profiles.html>`_
   * - `SUEWS_Snow <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Snow.html>`_ 
     - `SUEWS_Soil <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Soil.html>`_
     - 
     - `SUEWS_Snow <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Snow.html>`_ 
   * - `SUEWS_Profiles <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Profiles.html>`_
     - `SUEWS_Water <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Water.html>`_
     - 
     - `SUEWS_WithinGridWaterDist <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_WithinGridWaterDist.html>`_
   * - 
     - `SUEWS_Veg <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_Veg.html>`_
     - 
     - 
   * - `SUEWS_SiteSelect <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_SiteSelect.html>`_
     - `SUEWS_SiteSelect <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_SiteSelect.html>`__
     - `SUEWS_SiteSelect <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_SiteSelect.html>`_
     - `SUEWS_SiteSelect <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/SUEWS_SiteSelect.html>`_
      
      



 

Initial Conditions
==================

- `Initial conditions <https://suews.readthedocs.io/en/latest/input_files/Initial_Conditions/Initial_Conditions.html>`_

- Conducting a model spinup for a number of years allows for the influence of the conditions selected to begin with to become less critical.
- Key conditions to consider 
  
   - leaf area index (leaf-on, leaf-off) - this is critical for evaporation
   - soil moisture state - this is critical for evaporation
   
- less critical
  
   - surface state (as long as modelling for many days) as these will change rapidly. 
   - it is easy to just set this to be dry (e.g. summer) or wet (e.g. if rain has just occured)
   
- meteorological variables

   -  These can be determined from a wide range of data (e.g. the same source as your forcing data)
   
- snow conditions
 
   - This needs to be done very carefully for a short model run.  A long model run starting from snow-free conditons would ensure that the snow accumulation occurs at the right time etc
 
