# Completeness-Corrected Absorber Statistics from a Quasar Catalogue

This package enables the calculation of the number of absorbers per unit redshift (dN/dz) and per unit comoving pathlength (dN/dX), with built-in support for completeness correction on a pixel-by-pixel basis across a catalog of quasar spectra.

It seamlessly incorporates robust uncertainty estimation via bootstrapping, based on the typical pixel scale of absorber detections. These uncertainties are propagated through the completeness calculation and carried forward into the final estimates of (dN/dz) and (dN/dX).

The completeness calculation employs a novel variation of a commonly used method, designed to more accurately reflect the physical and statistical motivations relevant to large-scale astrophysical surveys.

## Overview

In Astrophysics quantifying the number of absorbers at varying redshifts provides crucial insights into the evolution of galaxies. One of the central methods for accomplishing this is to use down-the-barrel analysis of high redshift quasars to probe intervening elements. Quasars (galaxies with active galactic nuclei, AGN) are some of the brightest objects in the Universe, and have a characterings power law distribution of their flux as a function of wavelength. As light from these objects traverses the universe until it reaches our detectors it can be absorbed by intervening molecular clouds that are predominantly in the circumgalactic and intergalactic media (CGM and IGM). This absorption creates dips in the characteristic flux profile of the quasars. By studying these dips we can infer the number of such molecular clouds, the redshift (distance from us and age of the Universe where it is found), and through further analysis column density can also be inferred. These clouds can have temperatures well below that required for emission and are as such intrinsically very faint. Down-the-barrel analysis gives an emission, column density, and distance independent method for analyzing these clouds, and is therefore a crucial valuable method for learning about the Universe particularly at high redshift.

The number of absorbers per unit redshift (dN/dz) and per unit comoving pathlength (dN/dX) succinctly summarize many steps of down-the-barrel analysis, and quite involved. This code provides the function required to get such values and handles the associated uncertainties in a very robust way.

The package works in two parts; catalog completeness calculations, and calculation of dN/dz and dN/dX.

📘 See the full math-formatted notebook for completeness: [completeness_motivation.ipynb](completeness_motivation.ipynb)

📘 See the full math-formatted notebook for dN/dz and dN/dX: [dNdz_motivation.ipynb](coming  soon)


## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Repository Structure](#repository-structure)
- [License](#license)


## Installation

Clone the repository and install the required packages:

## Dependencies

This project requires the following Python packages:

- **pandas** — DataFrame manipulation and I/O
- **numpy** — Numerical computations
- **matplotlib** — Plotting and visualization
- **tqdm** — Progress bars for loops
- **scipy** — Interpolation and scientific utilities
- **astropy** — FITS file handling and statistical tools
- **json** — Built-in library for reading/writing JSON
- **pickle** — Built-in module for object serialization
- **os** — Standard library for file and directory operations

To install the required external packages, run:

```bash
pip install pandas numpy matplotlib tqdm scipy astropy
```

## Repository Structure

structure

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.











