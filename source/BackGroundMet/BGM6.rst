.. _QS:

**Storage Heat Flux**


The storage heat flux :math:`\Delta Q_S` is the net energy stored or released by changes in sensible heat within the canopy air layer, roughness elements (e.g. vegetation, buildings in an urban environment), and the ground.
Knowledge of :math:`\Delta Q_S` is crucial to a wide range of processes and applications: from modelling turbulent heat transfer and boundary layer development to predicting soil thermal fields.

In rural sites, or simple bare soil sites, the flux may be a small fraction of the net all-wave radiation (Oliphant et al., 2004).
However, in areas where there is more mass, such as cities, the term becomes much more significant ( `Kotthaus and Grimmond, 2014a <https://doi.org/10.1016/j.uclim.2013.10.002>`_ ) and a key element of the SEB and well-known effects such as the urban heat island.


**Objective Hysteresis Model**


The objective hysteresis model (OHM) is a simple model to calculate storage heat flux using net all-wave radiation :math:`Q^*` following the hysteresis relation (Camuffo and Bernardi, 1982).

The OHM is forced by :math:`Q^∗` and accounts for the diversity of the surface materials (sub-facets) in the measurement source area of interest with weightings (:math:`f`) for their two- or three-dimensional extent (Grimmond et al., 1991):

.. math::
  :label: ohm

  \Delta Q_{\mathrm{S}}=\sum_{i} f_{i}\left(a_{1, i} Q_{i}^{*}+a_{2, i} \frac{\partial Q_{i}^{*}}{\partial t}+a_{3, i}\right)

where the :math:`a_1`, :math:`a_2`, and :math:`a_3` coefficients are for individual facets determined by least-square regression between :math:`\Delta Q_S` and :math:`Q^*` using results from observations.

These coefficients capture the net behaviour of a facet type in a typical setting, rather than being required to identify the component materials within a facet (e.g. multiple materials making up a roof, wall, with varying thermal connectivity and individual properties). A set of example OHM coefficients can be found `here. <https://suews.readthedocs.io/en/latest/input_files/SUEWS_SiteInfo/Typical_Values.html#ohm-coefficients>`_

