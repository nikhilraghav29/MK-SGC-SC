# MK-SGC-SC: MULTIPLE KERNEL GUIDED SPARSE GRAPH CONSTRUCTION IN SPECTRAL CLUSTERING FOR UNSUPERVISED SPEAKER DIARIZATION 
### About
This repository contains the implementation for the paper:  
- " Nikhil Raghav, Avisek Gupta, Swagatam Das, and Md Sahidullah, *MK-SGC-SC: Multiple Kernel Guided Sparse Graph Construction in Spectral Clustering for Unsupervised Speaker Diarization*, communicated to ICASSP 2026.

## Instructions for implementation
Our implementation is based on a modified version of the AMI recipe provided in the SpeechBrain toolkit.
Use the following command to launch an experiment from your directory where your experiment.py is present. Consider the following as a case for launching the experiments on the AMI meeting corpus: 
- python experiment_ami.py hparams/ecapa_tdnn_ami.yaml

## Dependencies
Install speechbrain version 0.5.14
- Follow the installation guidelines for the SpeechBrain toolkit provided [here](https://github.com/speechbrain/speechbrain "SpeechBrain toolkit link")
## Recipe 
The following three files need to be overwritten at the following locations, depending on which speech corpora you want to perform the experiments among the DIHARD-III, AMI, and VoxConverse  datasets. 
It contains the scripts for the proposed MK-SGC-SC technique.

For example, if you want to experiment on the AMI meeting corpus, replace the files at the following locations:
- experiment.py located at speechbrain/recipes/AMI/Diarization with experiment_ami.py located at speechbrain/recipes/AMI/Diarization
- ecapa_tdnn.yaml located at speechbrain/recipes/AMI/Diarization/hparams with ecapa_tdnn_ami.yaml  speechbrain/recipes/AMI/Diarization/hparams
- diarization.py located at speechbrain/speechbrain/processing with diarization_amy.py located at speechbrain/speechbrain/processing
  
Similarly, you can do the experiments on DIHARD-III and VoxConverse.

## License
This project is licensed under the MIT License. The full terms of the MIT License can be found in the LICENSE.md file at the root of this project.

