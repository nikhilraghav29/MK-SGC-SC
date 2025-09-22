# MK-SGC-SC: MULTIPLE KERNEL GUIDED SPARSE GRAPH CONSTRUCTION IN SPECTRAL CLUSTERING FOR UNSUPERVISED SPEAKER DIARIZATION 
### About
This repository contains the implementation for the paper:  
- "Raghav, Nikhil and Gupta, Avisek, Das, Swagatam and Sahidullah, Md, *MK-SGC-SC: MULTIPLE KERNEL GUIDED SPARSE GRAPH CONSTRUCTION IN SPECTRAL CLUSTERING FOR UNSUPERVISED SPEAKER DIARIZATION*, communicated to ICASSP 2026.

## Instructions for implementation
Our implementation is based on a modified version of the AMI recipe provided in the SpeechBrain toolkit.
## Dependencies
Install speechbrain version 0.5.14
- Follow the installation guidelines for the SpeechBrain toolkit provided [here](https://github.com/speechbrain/speechbrain "SpeechBrain toolkit link") 
## Recipe 
The following three files need to be overwritten in the AMI recipe. The scripts were adapted for the experiments on the DIHARD-III dataset, AMI, and VoxConverse speech corpora. It contains the scripts for the proposed MK-SGC-SC technique:
- experiment.py located at /speechbrain/recipes/AMI/Diarization/experiment_ami.py
- ecapa_tdnn.yaml located at /speechbrain/recipes/AMI/Diarization/ecapa_tdnn_ami.yaml
- diarization.py located at /speechbrain/speechbrain/processing/diarization_ami.py

## License
This project is licensed under the MIT License. The full terms of the MIT License can be found in the LICENSE.md file at the root of this project.

