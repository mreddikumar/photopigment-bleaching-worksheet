# Photopigment Bleaching Worksheet

A quantitative photometric and radiometric framework for simulating retinal photopigment bleaching under brief flash stimulation.

This repository contains a Jupyter notebook implementing:

- First-order exponential bleaching model 
- Retinal illuminance (Trolands) calculations  
- Radiant power ↔ bleach % inversion  
- Photon count and photon density computation  
- CIE 1931 photopic luminous efficiency integration  


## Overview

The notebook provides two equivalent computational routes:

1. **Photometric (Troland-based) formulation**
2. **Radiometric (photon-based) formulation**

Users can input:

- Wavelength (nm)  
- Flash duration (ms)  
- Retinal stimulus diameter (µm)  
- Nodal distance to retina (mm)  
- Target bleaching percentage  

The notebook computes:

- Required radiant power (µW)  
- Forward bleach verification  
- Total photon count  
- Photon density (photons/µm²)  

All equations and derivations are documented directly inside the notebook.


## Data Source

Photopic luminous efficiency values are taken from:

Commission Internationale de l'Éclairage (CIE)  
CIE spectral luminous efficiency for photopic vision (CIE 1931 standard observer)  
CIE S 026/E:2018 dataset  https://cie.co.at/datatable/cie-spectral-luminous-efficiency-photopic-vision  


## Key References

Rushton WA, Henry GH.  *Bleaching and regeneration of cone pigments in man.*  Vision Research, 1968.

Packer O, Williams DR. *Light, the retinal image, and photoreceptors.* In: Shevell SK (ed.), The Science of Color. Elsevier; 2003:41–102.

Thibos LN. *What is a troland?* JOSA A, 2018.

Vienola KV, Valente D, Zawadzki RJ, Jonnal RS. Velocity-based optoretinography for clinical applications. Optica. 2022;9(10):1100–1108. https://doi.org/10.1364/optica.460835  


## Requirements

- Python 3.x  
- NumPy  
- Pandas  
- Jupyter Notebook  


## Usage

1. Open the notebook.
2. Run all cells sequentially.
3. Enter stimulus parameters when prompted.
4. Review computed bleaching and photon metrics.


## Notes

- 100% bleach is mathematically undefined (logarithmic divergence).
- All geometric assumptions follow small-angle retinal projection.
- Ocular transmission is assumed to be unity unless otherwise specified.


## Authors

**Reddikumar Maddipatla**$^{1,2}$, **Robert J. Zawadzki**$^{1,2}$, and  **Ravi S. Jonnal**$^{1}$  

$^{1}$ Center for Human Ophthalmic Imaging Research (CHOIR), UC Davis Eye Center, Sacramento, CA 95817, USA  

$^{2}$ EyePOD Imaging Lab, Department of Cell Biology and Human Anatomy, University of California, Davis, CA 95616, USA


