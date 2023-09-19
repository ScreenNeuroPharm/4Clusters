# CxHp-2D
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ScreenNeuroPharm/4Clusters/blob/master/LICENSE)

> The repository contains the data and the functions need to reproduce the analysis reported in the article "Multiple neuron clusters on Micro-Eelectrode Arrays as an in vitro model of brain network".

## Details
All uploaded scripts work with a .mat format. 
To reproduce our analysis is necessary to convert the ```.txt``` format file in ```.mat``` format file using the function ```TxT2Mat.m``` in the folder Conversion. 
All electrophysiological recordings are sampled at 10 KHz. 
```TxT2Mat.m``` function allows obtaining for each electrode (60) the peak train .mat file. 
Peak_train file is a sparse vector that reports the spike occur, saving the spike amplitudute.

### Code folder architecture:
- BurstAnalysis folder:
    * burstFeaturesAnalysis: functions to obtain the burst feautures
    * StringMethod: functions to detect the burst

- Conversion folder:
    * Txt2Mat: function to convert ```.txt``` format file in ```.mat``` format file

- NetworkBurstAnalysis folder: 
    * IBEi: functions to extract the Inter Burst Event interval (threshold used to detect the Network Burst)
    * NBPropagation: function to analyse the Network Propagation
    * NetBurstDetection: functions for the Network Burst Detection

- SpikeAnalysis folder:
    * MFR: function to compute the Mean Firing Rate
	


- Utilities folder: supplementary functions
