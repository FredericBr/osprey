# Osprey

Osprey is an all-in-one software suite for state-of-the art processing and
quantitative analysis of in-vivo magnetic resonance spectroscopy (MRS) data.

### Features
- 1-file job definition system for reproducible data analysis
- Automated recognition of input file format and sequence origin
- Fully-automated loading and pre-processing pipeline for optimal SNR, linewidth, phasing, and alignment
- Integrated linear-combination modeling module
- Full density-matrix simulated basis sets (using real pulses and sequence timings; including effects of localization and spectral editing) for many metabolites and common sequence implementations
- Functions to create custom basis sets and import basis sets from LCModel or Tarquin
- Integrated voxel co-registration and segmentation module (requires SPM12)
- Quantification based on tissue fractions and (customizable) metabolite/tissue water relaxation times
- GUI to display data, quality assessment, and quantitative results at each step of the analysis
- Rich 'Overview' GUI panel for batched datasets to visualize distributions of metabolite estimates and mean +/- SD spectra

### Supported methods
- Conventional MRS (STEAM, PRESS, semi-LASER, LASER)
- MEGA editing
- Hadamard-encoded editing (HERMES, HERCULES)

### Supported sequence implementations
- Philips (Philips product sequences; Johns Hopkins patches)
- Siemens (Siemens product and WIP sequences; Johns Hopkins patches; CMRR sequences; Jamie Near sequence)
- GE (GE product sequences; Ralph Noeske sequence)

### Supported file formats
- Philips: SDAT/SPAR, DATA/LIST (coming soon), SIN/LAB/RAW (coming soon)
- Siemens: TWIX/DAT, RDA (single- & multi-file), DICOM (DCM/IMA, single- & multi-file)
- GE: P

## Getting started

### Prerequisites

Osprey requires [MATLAB](https://www.mathworks.com/products/matlab.html) and
has been tested on version 2017a and newer. The following toolboxes are
required for full functionality:

- Image processing
- Optimization
- Signal Processing
- Statistics and Machine Learning
- Curve Fitting Toolbox

### Installation

Download the latest **Osprey** code from its [GitHub
repository](https://github.com/schorschinho/osprey), then extract and add the
entire folder (with subfolders) to your MATLAB path. Make sure to regularly
check for updates, as we frequently commit new features, bug fixes, and improved
functions.

To perform voxel co-registration and tissue segmentation, download **SPM12**
[from the UCL website](http://www.fil.ion.ucl.ac.uk/spm/software/spm12/), then
extract and add to your MATLAB path.

If you want to use the `Osprey` Graphical User Interface (GUI),
please download the following toolboxes from the MATLAB File Exchange:

- [GUI Layout Toolbox](https://www.mathworks.com/matlabcentral/fileexchange/47982-gui-layout-toolbox)
      (David Sampson)

- [Widget Toolbox](https://www.mathworks.com/matlabcentral/fileexchange/66235-widgets-toolbox)
      (Robin Jackey)

Download both toolboxes in the MATLAB toolbox format (.mltbx). You can
double-click to install. MATLAB will automatically add the toolboxes to its
path.

## Contact, Feedback, Suggestions

For any sort of questions, feedback, suggestions, or critique, please reach out to us via gabamrs@gmail.com. We also welcome your direct contributions to Osprey here in the GitHub repository.

## Developers

- [Georg Oeltzschner](mailto:goeltzs1@jhu.edu)
- [Helge J. Zöllner](mailto:hzoelln2@jhu.edu)
- [Richard A. E. Edden](mailto:raee2@jhu.edu)

Should you publish material that made use of Osprey, please cite the following publication:

[G Oeltzschner, HJ Zöllner, SCN Hui, M Mikkelsen, MG Saleh, S Tapper, RAE Edden. Osprey: Open-Source Processing, Reconstruction  & Estimation of Magnetic Resonance Spectroscopy Data. bioRxiv 2020.](https://www.biorxiv.org/content/10.1101/2020.02.12.944207v1)

## Acknowledgements

We wish to thank the following individuals for their contributions to the
development of Osprey and shared processing code:

- Jamie Near (McGill University, Montreal)
- Ralph Noeske (GE Healthcare, Berlin)
- Peter Barker (Johns Hopkins University, Baltimore)
- Robin de Graaf (Yale School of Medicine, New Haven)
- Philipp Ehses (German Center for Neurodegenerative Diseases, Bonn)
- Wouter Potters (UMC Amsterdam)

This work has been supported by NIH grants R01EB016089, P41EB15909, R01EB023963, and K99AG062230.
