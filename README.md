# mcw_Preclinical_MRIsequences
Public-facing repository for various MRI pulse sequences developed by M Budde at the Medical College of Wisconsin. 
This repository is replacement for the previous [OSF sharing site](https://osf.io/ngu4a/)

Code and binaries are contained within individual private repositories.

For access to individual sequences and versions, please follow the instructions in this [discussion](https://github.com/mdbudde/mcw_Preclinical_MRIsequences/discussions/1), or email mdbudde@mcw.edu.


## DWWave: Diffusion encoding with arbitrary waveforms. 
Original shared sequences for arbitrary diffusion gradient waveforms selectable through the user interface. This version has been used by 40+ investigators and updated extensively based on user feedback.
- [mcw_DWWaveEPIv7_PV6](https://github.com/mdbudde/mcw_DWEpiWavev7_PV6) 
- mcw_DWWaveEPIv7_PV7
- [mcw_DWWaveEPIv7_PV360.1.1](https://github.com/mdbudde/mcw_DWEpiWavev7_PV360.1.1)
- mcw_DWWaveStanv7_PV6
- mcw_DWWaveStanv7_PV7
- <ins>For newer PV360 versions (v3.#)</ins>, please let me know if you are interested in collaborating. It is generally trivial to update methods, but I don't have direct access for compilation and testing and don't want to release untested code. 
![image](https://github.com/user-attachments/assets/44f55daf-435b-4240-b972-82a5387f5f6d)


New variant that replaces the user interface with a formatted text file for full customization of gradient shapes, amplitude, direction. It has not been tested beyond simulations and is available to users wishing for more flexibility but may require careful evaluation of the acquisition and results. 
- [mcw_DWWaveEPIv8_PV6](https://github.com/mdbudde/mcw_DWEpiWavev8)
![image](https://github.com/user-attachments/assets/3f6a6ab2-50d8-4aa0-9869-1b6bee326687)


## DWBIR-RARE: Diffusion prepared Fast Spin Echo (RARE). 
A B1-insensitive adiabatic module (BIR4 or BIR8) with diffusion preparation under different motion-compensation conditions (M0, M1, M2) is coupled with a fast spin echo readout to minimize motion and susceptibility artifacts. Pulses are included and custom gradient tables can be loaded from a file. Lee SL et al. MRM 2021
- Please inquire if interested.
![image](https://github.com/user-attachments/assets/26ecc9b5-8551-4ec4-b85b-3402847c09d1)

## vfaRARE: variable flip angle RARE sequence
High resolution, efficient 3D imaging (Note more recent versions of Paravision include their implementation of this method).
Distortion-free imaging
100+ echoes per excitation.
T2 contrast
- Please inquire if interested.
- ![image](https://github.com/user-attachments/assets/c87d5f32-617c-4d8e-af98-2faf4e160b5a)




## pCASL: Pseudocontinuous ASL sequences (Binary version only)
A RARE (FSE) version is available with an embarrassingly large number of options and settings that were used for optimization and various experiments. Besides the typical settings for labelling settings/durations/delays, it includes Hadamard options, many different background suppression options, triggered labelling/delays, dynamic shimming, multiple references for M0/T1 mapping, vessel and/or spatial suppressions. Only the single-slice 2D setup has been well-tested, although others are available.
The FLASH version is similar but with fewer options, but also includes multiple repetitions or movie mode, with the same k-space line acquired multiple times after the labeling for dynamic studies.
- Please inquire if interested.
