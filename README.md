# mcw_Preclinical_MRIsequences
Public-facing repository for various MRI pulse sequences developed by M Budde at the Medical College of Wisconsin. 
This repository is a newer extension of a previous OSF sharing site: https://osf.io/ngu4a/


List of sequences:
DWIWave: Diffusion encoding with arbitrary waveforms. Both EPI and spin-echo versions are available. See the associated quickstart for installation and detailed usage. Also includes:


dtiEpi_GRFat: DTI-EPI version with 2 additional options:
gradient reversal fat saturation for improved fat suppression
Reversed blip phase encoding for distortion correction


DWBIR-RARE: Diffusion prepared Fast Spin Echo (RARE). A B1-insensitive adiabatic module (BIR4 or BIR8) with diffusion preparation under different motion-compensation conditions (M0, M1, M2) is coupled with a fast spin echo readout to minimize motion and susceptibility artifacts. Pulses are included and custom gradient tables can be loaded from a file. Lee SL et al. MRM 2021


vfaRARE: variable flip angle RARE sequence for high resolution 3D imaging (Note more recent versions of Paravision include their implementation this method).
distortion-free imaging
100+ echoes per excitation.
T2 contrast



pCASL: Pseudocontinuous ASL sequences (Binary version only)
A RARE (FSE) version is available with an embarrassingly large number of options and settings that were used for optimization and various experiments. Besides the typical settings for labelling settings/durations/delays, it includes Hadamard options, many different background suppression options, triggered labelling/delays, dynamic shimming, multiple references for M0/T1 mapping, vessel and/or spatial suppressions. Only the single-slice 2D setup has been well-tested, although others are available.
The FLASH version is similar but with fewer options, but also includes multiple repetitions or movie mode, with the same k-space line acquired multiple times after the labeling for dynamic studies.
