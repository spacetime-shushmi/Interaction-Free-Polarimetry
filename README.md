# Interaction-Free-Polarimetry
Code accompanying paper on interaction-free polarimetry. It simulates the protocol, calculates detection and absorption probabilities, fits the sample parameters, reconstructs sample Mueller matrices and analyses the signal-to-noise ratio (SNR).
# Interaction-Free Polarimetry

This repository contains the Python code accompanying our work on interaction-free polarimetry. The code simulates the polarimetry protocol using a density matrix formalism and investigates the reconstruction of the polarisation properties of diattenuating samples.

## Overview

The notebook (Polarimetry_Protocol_Diattenuation.ipynb) includes:

- Preparation of six input polarisation states (H, V, D, A, R and L) through heralding.
- Simulation of the interferometer for different numbers of cycles and sample parameters.
- Calculation of the output Stokes parameters, detection probabilities and absorption probabilities.
- Reconstruction of the sample's Mueller matrix and evaluation of reconstruction errors.
- Physicality checks of the reconstructed Mueller matrices using Choi matrix representation.
- Analysis of absorption probability and detector contrast as functions of the number of cycles and sample attenuation.
- Calculation of the signal-to-noise ratio (SNR), normalised by the square root of the mean number of incident and absorbed photons.
- Generation of figures, heatmaps and tables.

The simulations assume ideal optical components (apart from the sample) and detectors. The Mueller matrix reconstruction examples use simulated data without added counting noise and assume zero relative phase between the principal axes.

## Requirements

- Python 3
- NumPy
- SciPy
- Matplotlib
- Pandas
- Jupyter Notebook
- LaTeX (for figure rendering)

## Usage

Open the notebook in Jupyter and run the cells sequentially. The sample transmissions, orientation, input polarisation and number of interferometer cycles can be modified to investigate different sample configurations.
