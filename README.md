# Ach-phfMRI

This repository contains codes and data in support of the paper (tentative) "Pharmacological meta-analysis of cholinergic modulation on attention" 

## Publications

{Link to preprint DOI, publication DOI once it's ready...}

## Data

Contains the following data file necessary to run the analysis provided in the notebooks.\
**HCP-MMP1 annot files**: *{lh,rh}_HCP-MMP1_fsa10.annot* - HCP-MMP1 parcellation annotation files in fsa-10k space for [brainspace](https://brainspace.readthedocs.io/en/stable/index.html) visualization.\
**Glasser 360 fsa5 label files**:_glasser_360_fsaverage5_{lh,rh}label.gii_ - Glasser parcellation labels in fsa10k for parcellating whole brain data (such as the geodesic, myelin and FEOBV data).\
**BF surface label**:_seed-BASF.{L,R}.bin.fsa5.shape.gii_ - basal forebrian (BF) seed label in surface space (see Methods section of the publication for the details of creating this file).\
**FEOBV PET imaging data**:_t2a_wProject_TWS_001_FEOBV_pvcwac_1-13.nii_ -  [¹⁸F]fluoroethoxybenzovesamicol ([18F]FEOBV) imaging data targeting the vesicular acetylcholine transporter (VAChT) protein ([Kanel, van der Zee, Sanchez-Catasus, et al., 2022](https://www.sciencedirect.com/science/article/pii/S2589958922000111)) used to compare with the meta-analysis connectivity maps.\
**BF cortical connectivity map**:_Parc-Inv-rescaled_metric-average_{L,R}_fsa-10k.shape.gii_ - cortical surface map of intrinsic BF cortical connectivity ref: [Human Basal Forebrain (BF) Multimodal Connectivity](https://github.com/sudesnac/HumanBF-Connectivity). 
Reference surface for fsa-10k can be downloaded from [here](https://github.com/MICA-MNI/BrainSpace/tree/master/brainspace/datasets/surfaces) for visualizing gii files using workbench.\
**Meta-analysis connectivity maps**:_AG*.nii(s)_ and *{NbM,NbMSep}_18apr2023_MACM_Z.nii* - output connectivity maps (in nii) of the meta-analysis. \
*AG_increase_18apr2023_{ALE,C05_5k_ALE,Z}.nii* : [add specifics] \
*AG_decrease_18apr2023_C05_5k_ALE.nii* : [add specifics] \
*AG_decrease_18apr2023_MACM_{C05_5k_ALE,Z}.nii* : [add specifics] \
*AG_merge_18apr2023_MACM_{C05_5k_ALE,Z}.nii* : [add specifics] \
*{NbM,NbMSep}_18apr2023_MACM_Z.nii*: [add specifics]


## Code

Text files (.txt) tables that can be used as the input files for running meta-analysis using [gingerALE](http://www.brainmap.org/ale/). 

## Notebook

### spin-tests.ipynb
The jupyter notebook for running the codes to transform the nii data into cortical surface data, run spin tests analyses, and create the figures used in this paper.
### Visualize_MACM.ipynb
The jupyter notebook to load the MNI coordinates of the meta-analysis and visualize in 3D glass brain (saved as .html files in figures).


## Results

This folder contains the csv files of cortical surface converted and rescaled meta-analysis connectivity maps (both rescaled whole brain and parcellated rescaled). 
as well as the csv files from the results of [Human Basal Forebrain (BF) Multimodal Connectivity](https://github.com/sudesnac/HumanBF-Connectivity).

## figures

This folder contains the figures created.
