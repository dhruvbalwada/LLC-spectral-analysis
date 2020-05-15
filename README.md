# Earth-Cube-2020-spectral-analysis
Repo with notebooks showing how to use xrft to do spectral analysis of LLC4320.

[![Binder](https://binder.pangeo.io/badge_logo.svg)](https://binder.pangeo.io/v2/gh/dhruvbalwada/Earth-Cube-2020-spectral-analysis/master)

# Spectral Analysis using xrft and Pangeo
**Dhruv Balwada, Takaya Uchida, and Ryan Abernathey**  
*University of Washington,  
Institut des Géosciences de l'Environnement, and  
Columbia University*  
Contact: dbalwada@uw.edu

**Abstract**
 >Turbulent flows, such as the macroscale chaotic flows of the ocean and atmosphere, are inherently multiscale phenomena. With the advancements in computational power and modern satellite observational platforms, we are able to generate model and observational fields that are able to sample the evolution of these turbulent flows. Spectral analysis of these turbulent flows is an extremely powerful tool that allows us to glean a deeper fundamental understanding of how the turbulence transfers and equilibrates energy and tracers across scales, or simply put helps us understand how do flow structures grow and decay?  
Turbulence resolving data sets are generally large in size due to high spatial and temporal resolution requirements to sample the rapidly evolving turbulent flows. This poses a unique challenge for the computation of the spectral properties of these fields. In this notebook we leverage a python toolbox - xrft (https://xrft.readthedocs.io/), which is part of the Pangeo (https://pangeo.io/) stack, along with the resources of Pangeo cloud to demonstrate how spectral calculations can be carried out efficiently. Xrft leverages the existing architecture of xarray, which allows the tracking of its metadata (i.e. spatial and temporal coordinates), and dask, which allows automatic parallelization, to easily and rapidly calculate discrete fourier transforms, while tracking the metadata of the variables. In particular, we show how to use xrft to estimate the power spectra, cross-spectra and spectral transfer rates of variables in a submesoscale resolving ocean simulation. However, the tools and workflows are general and can easily be extended to other simulation outputs and satellite based surface fields.
