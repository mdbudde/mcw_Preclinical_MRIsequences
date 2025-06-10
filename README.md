# mcw_Preclinical_MRIsequences
Public-facing repository for various MRI pulse sequences developed by M Budde at the Medical College of Wisconsin. 
This repository is replacement for the previous [OSF sharing site](https://osf.io/ngu4a/)

:bangbang: **To access sequences (private repositories), follow these [instructions](https://github.com/mdbudde/mcw_Preclinical_MRIsequences/discussions/1), or email mdbudde@mcw.edu with your github username and desired sequence version.** :bangbang:


## DWWave: Diffusion encoding with arbitrary waveforms. 
Original shared sequences for arbitrary diffusion gradient waveforms selectable through the user interface. This version has been used by 40+ investigators and updated extensively based on user feedback.
- [mcw_DWEpiWavev7_PV6](https://github.com/mdbudde/mcw_DWEpiWavev7_PV6) 
- mcw_DWEpiWavev7_PV7
- [mcw_DWEpiWavev7_PV360.1.1](https://github.com/mdbudde/mcw_DWEpiWavev7_PV360.1.1)
- mcw_DWWaveStanv7_PV6
- mcw_DWWaveStanv7_PV7
- [mcw_DWEpiWavev7_PV360.3.6](https://github.com/mdbudde/mcw_DWEpiWavev7_PV360.3.6)   Programmed but uncompiled/untested. Please let me know if you are interested in collaborating; I don't have direct access for compilation and testing. 
<img width="550" alt="image" src="https://github.com/user-attachments/assets/44f55daf-435b-4240-b972-82a5387f5f6d" />



- [mcw_DWEpiWavev8_PV6](https://github.com/mdbudde/mcw_DWEpiWavev8)
  New variant that replaces the user interface with a formatted text file for full customization of gradient shapes, amplitude, direction. It has been tested in simulations and is available to users desiring for more flexibility but may require careful evaluation of the acquisition and results. 
<img width="550" alt="image" src="https://github.com/user-attachments/assets/3f6a6ab2-50d8-4aa0-9869-1b6bee326687" />

```
# DWITABLE: list of scans/images with shape, direction, and amplitude for each
# NUM SHAPE1_ID SHAPE2_ID DIR_ID AMP
  # b=0
  1   1   1    1     0
  # different directions
  2   1   1    2     80
  # different amplitudes
  3   1   1    2     20
  # different shapes
  4   2   2    1     80
...
### DIRECTIONS: list of directions that are indexed from dwitable
# DIR_ID X Y Z 
  1 0 0 1
  2 1 0 0
  3 1 1 0
  ...
### SHAPES: gradient waveforms are stored as arrays in the same file
shape_id 1
shape_label stick
origin_vect 0 0 1 
duration 0.008
num_samples 1000
0.000000 0.000000 0.000000
0.000000 0.000000 0.013289
...
shape_id 2
shape_label sphere
origin_vect 0 0 1 
duration 0.008
num_samples 1000
0.000000 0.000000 0.000000
0.010851 0.000000 0.007673
...

### OUTPUT: Will write scan info (shape/rotations/amplitudes, or b-matrices?) at the bottom of this file when the sequence runs.
#To facilitite processing without extracting from parameter files. 
#NUM SHAPE1_ID SHAPE2_ID AMP R00 R01 R02 R11 R12 R22

```

## DWBIR-RARE: Diffusion prepared Fast Spin Echo (RARE). 
A B1-insensitive adiabatic module (BIR4 or BIR8) with diffusion preparation under different motion-compensation conditions (M0, M1, M2) is coupled with a fast spin echo readout to minimize motion and susceptibility artifacts. Pulses are included and custom gradient tables can be loaded from a file. [Lee SL et al. MRM 2021](https://pubmed.ncbi.nlm.nih.gov/33720450/)
- Please inquire if interested.
- <img width="550" alt="image" src="https://github.com/user-attachments/assets/26ecc9b5-8551-4ec4-b85b-3402847c09d1" />

## vfaRARE: variable flip angle RARE sequence
High resolution, efficient 3D imaging (Note more recent versions of Paravision include their implementation of this method).
Distortion-free imaging
100+ echoes per excitation.
T2 contrast
- Please inquire if interested.
- <img width="550" alt="image" src="https://github.com/user-attachments/assets/c87d5f32-617c-4d8e-af98-2faf4e160b5a" />




## pCASL: Pseudocontinuous ASL sequences (Binary version only)
A RARE (FSE) version is available with an embarrassingly large number of options and settings that were used for optimization and various experiments. Besides the typical settings for labelling settings/durations/delays, it includes Hadamard options, many different background suppression options, triggered labelling/delays, dynamic shimming, multiple references for M0/T1 mapping, vessel and/or spatial suppressions. Only the single-slice 2D setup has been well-tested, although others are available.
The FLASH version is similar but with fewer options, but also includes multiple repetitions or movie mode, with the same k-space line acquired multiple times after the labeling for dynamic studies. [Meyer B, et al, JCBFM 2021](https://pubmed.ncbi.nlm.nih.gov/33509036/) and [Lee ST et al, NMR Biomed 2024](https://pubmed.ncbi.nlm.nih.gov/38355219/)
- Please inquire if interested.
<img width="550" alt="image" src="https://github.com/user-attachments/assets/780f0800-e31b-4408-8262-9a69f2d7eb35" />


