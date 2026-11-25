
# Interaction-Free Polarimetry

Python code for our interaction-free polarimetry work. It simulates the protocol, works out detection and absorption probabilities, fits sample parameters, reconstructs Mueller matrices, and looks at signal-to-noise ratio (SNR).

## Notebooks

**Polarimetry_Protocol_Diattenuation.ipynb**
Runs the protocol for different numbers of cycles and sample parameters. It computes output Stokes parameters, detection and absorption probabilities, and reconstructs the sample's Mueller matrix along with the Frobenius errors. It also checks whether the reconstructed matrices are physical using the Choi matrix, and looks at SNR normalised by the square root of the mean incident and absorbed photon numbers.

**opaque_vs_transparent-sample.ipynb**
Uses the same framework to tell a fully opaque sample apart from no sample. It finds the attenuation where protocol absorption equals single-pass absorption, and runs the SNR analysis.

**Bound-retardance-depolarising.ipynb**
Extends the protocol to retarding and depolarising samples. It covers Fisher information and Cramér–Rao bounds, compares precision for equal incident and expected absorbed photons, and fits transmissions, axis orientation and retardance from noiseless simulated data. It also compares depolarisation Fisher information per incident photon and per sample pass.

**Note:** The simulations assume ideal optics and detectors, apart from the sample. The Mueller reconstruction examples use noiseless data and assume zero relative phase between the principal axes.

## Requirements

Python 3, NumPy, SciPy, Matplotlib, Pandas, Jupyter Notebook, and LaTeX (for figures).

## Usage

Open a notebook in Jupyter and run the cells in order. Can change the parameters and the number of interferometer cycles to try other sample setups.
