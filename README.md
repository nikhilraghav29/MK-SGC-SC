# MK-SGC-SC: MULTIPLE KERNEL GUIDED SPARSE GRAPH CONSTRUCTION IN SPECTRAL CLUSTERING FOR UNSUPERVISED SPEAKER DIARIZATION 
### About
This repository contains the implementation for the paper:  
- "Raghav, Nikhil and Gupta, Avisek, Das, Swagatam and Sahidullah, Md, *MK-SGC-SC: MULTIPLE KERNEL GUIDED SPARSE GRAPH CONSTRUCTION IN SPECTRAL CLUSTERING FOR UNSUPERVISED SPEAKER DIARIZATION*, communicated to ICASSP 2026.


## Dependencies
Our implementation is based on a modified version of the AMI recipe provided in the SpeechBrain toolkit.
- Follow the installation guidelines for the SpeechBrain toolkit provided [here](https://github.com/speechbrain/speechbrain "SpeechBrain toolkit link") 
## Method
The following three files were modified from the exisitng AMI recipe, and were adapted for the experiments on the DIHARD-III dataset. It contains, the scripts for the proposed SC-pNA technique:
- experiment.py located at /speechbrain/recipes/AMI/Diarization/experiment.py
- ecapa_tdnn.yaml located at /speechbrain/recipes/AMI/Diarization/ecapa_tdnn.yaml
- diarization.py located at /speechbrain/speechbrain/processing/diarization.py

## License
This project is licensed under the MIT License. The full terms of the MIT License can be found in the LICENSE.md file at the root of this project.

