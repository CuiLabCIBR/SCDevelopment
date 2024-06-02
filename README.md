# SCDevelopment
Data and codes for our paper "Structural connectivity matures along a sensorimotor-association connectional axis in youth".

Most codes were written in R, and a few in Matlab. The original data for these analyses are available via the NIMH Data Archive (NDA) [the Adolescent Brain Cognitive Development, (ABCD)](https://nda.nih.gov/abcd), [the Lifespan Human Connectome Project in Development (HCP-D)](https://nda.nih.gov/ccf)

## demopath
This folder contains the demographic, cognitive, and psychopathological characteristics of the participants in the ABCD and HCP-D datasets. `DemodfScreenFinal.csv` is for the ABCD dataset. `HCPD_demo_behav.csv` is for the HCP-D dataset. The codes for organizing these dataframes are located in `/development_script/1st_dataclean/merge_demography_info_and_screen`.

## wd
This folder contains statistical magnitudes, data for visualization and derivatives derived from the analyses. It has four sub-folders:
* [interdataFolder_ABCD](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/wd/interdataFolder_ABCD) : Statistical magnitudes derived from general additive mixed models (GAMM) or general additive models (GAM) fitted to the ABCD dataset.
* [interdataFolder_HCPD](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/wd/interdataFolder_HCPD) : Statistical magnitudes derived from GAM fitted to the HCP-D dataset. 
* [results_ABCD](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/wd/results_ABCD) : Derivatives and posterior derivatives of developmental GAMM fitted to the ABCD datasets, including correlation coefficients with posterior derivatives at 1,000 specific age points within the age span.
* [results_HCPD](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/wd/results_HCPD) : Derivatives and posterior derivatives of developmental GAM fitted in the HCP-D datasets, including correlation coefficients with posterior derivatives at 1,000 specific age points within the age span.

## development_script
This folder contains codes for all the analyses in the manuscript and the sensitivity analyses in the supplementary materials.

* The [1st_dataclean](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/development_script/1st_dataclean) folder contains codes to extract the structural connectivity (SC) strength of large-scale SC matrices and conduct ComBat analyses.
* The [2nd_fitdevelopmentalmodel](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/development_script/2nd_fitdevelopmentalmodel) folder contains codes to fit GAM or GAMM to evaluate developmental effects and compare the spatial patterns with the sensorimotor-association (S-A) connectional axis.
* The [3rd_plotConnectionalAxis](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/development_script/3rd_plotConnectionalAxis) folder contains codes to visualize the S-A connectional axis and S-A cortical axis.
* The [4th_changerate_SAcorr](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/development_script/4th_changerate_SAcorr) folder contains codes designed for age-resolved developmental analyses and separate analyses within datasets partitioned based on the age threshold where the alignment of developmental effects undergoes a reversal.
* The [5th_cognition](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/development_script/5th_cognition) folder contains codes to conduct cognitive analyses.
* The [6th_pfactor](https://github.com/XiaoyuXu750/SCDevelopment/tree/main/development_script/6th_pfactor) folder contains codes to conduct psychopathological analyses.

See the `README` in each folder for details of individual scripts.

## gamfunction
This folder contains functions called in the analyses. The functions called in the scripts in the `development_script` folder can be found here.

