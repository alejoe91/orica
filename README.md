# ORICA: Online Recursive Independent Component Analysis

This package implements the online recursive ICA algorithm [[1](http://ieeexplore.ieee.org/abstract/document/7355373/),[2](http://ieeexplore.ieee.org/abstract/document/6944462/)] for real-time adaptive blind source separation of high-density EEG data [[1](http://ieeexplore.ieee.org/abstract/document/7355373/),[3](http://ieeexplore.ieee.org/abstract/document/7319297/)]. ORICA was also implemented as functions in [BCILAB](https://sccn.ucsd.edu/wiki/BCILAB) and [EEGLAB](https://sccn.ucsd.edu/eeglab/index.php) and was integrated in an open-source [Real-time EEG Source-mapping Toolbox (REST)](https://github.com/goodshawn12/REST "REST"), supporting applications in ICA-based online artifact rejection, feature extraction for real-time biosignal monitoring in clinical environments, and adaptable classifications in brain-computer interfaces.


### Motivation
Independent Component Analysis (ICA) has been widely applied to electroencephalographic (EEG) biosignal processing and brain-computer interfaces. The practical use of ICA, however, is limited by its computational complexity, data requirements for convergence, and assumption of data stationarity, especially for high-density data. Hence we develop an optimized online recursive ICA algorithm (ORICA) with online recursive least squares (RLS) whitening for blind source separation of high-density EEG data, which offers instantaneous incremental convergence upon presentation of new data. 


### To use ORICA
* See [testScript.m](testScript.m) for example codes of running ORICA.
* Use EEGLAB for performance evaluation. EEGLAB can be downloaded at [Bitbucket](https://bitbucket.org/sccn_eeglab/eeglab)


### Files description
- testScript.m		- Example script that shows how to run ORICA.
- SIM_STAT_16ch_3min.set 	- A simulated EEG data with 16-channel and 3-min with sampling rate 128 Hz, generated by random-coefficients autoregressive model. 


### References
[1] S.-H. Hsu, T. Mullen, T.-P Jung, and G. Cauwenberghs, "[Real-time adaptive EEG source separation using online recursive independent component analysis](http://ieeexplore.ieee.org/abstract/document/7355373/)," IEEE Transactions on Neural Systems and Rehabilitation Engineering, 2016.

[2] S.-H. Hsu, T. Mullen, T.-P Jung, and G. Cauwenberghs, "[Online recursive independent component analysis for real-time source
separation of high-density EEG](http://ieeexplore.ieee.org/abstract/document/6944462/)," in IEEE EMBS, 2014.

[3] S.-H. Hsu, L. Pion-Tanachini, T.-P Jung, and G. Cauwenberghs, "[Tracking non-stationary EEG sources using adaptive online 
recursive independent component analysis](http://ieeexplore.ieee.org/abstract/document/7319297/)," in IEEE EMBS, 2015.

### Author
Sheng-Hsiou (Shawn) Hsu, SCCN, UCSD

For any question or potential collaboration, contact me at shh078 at ucsd dot edu.
