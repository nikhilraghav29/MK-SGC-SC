# MK-SGC-SC: Multiple Kernel Guided Sparse Graph Construction in Spectral Clustering for Unsupervised Speaker Diarization

### About
This repository contains the implementation for the paper:  
- Nikhil Raghav, Avisek Gupta, Swagatam Das, and Md Sahidullah, *MK-SGC-SC: Multiple Kernel Guided Sparse Graph Construction in Spectral Clustering for Unsupervised Speaker Diarization*, communicated to ICASSP 2026.

## Dependencies
Install SpeechBrain version `0.5.14`.
Follow the installation guidelines provided in the [SpeechBrain repository](https://github.com/speechbrain/speechbrain).

## Recipe 
This repository provides scripts for the proposed MK-SGC-SC technique.  
To run experiments on the **DIHARD-III**, **AMI**, or **VoxConverse** datasets, overwrite the following files in the SpeechBrain toolkit.

For example, for the **AMI meeting corpus**, replace:
- `speechbrain/recipes/AMI/Diarization/experiment.py` → `experiment_ami.py`
- `speechbrain/recipes/AMI/Diarization/hparams/ecapa_tdnn.yaml` → `ecapa_tdnn_ami.yaml`  
- `speechbrain/speechbrain/processing/diarization.py` → `diarization_ami.py`
  
Similarly, you can do the experiments on DIHARD-III and VoxConverse.

## Instructions for implementation
Our implementation is based on a modified version of the AMI recipe provided in the SpeechBrain toolkit.
Use the following command to launch an experiment from your directory where your experiment.py is present. Consider the following as a case for launching the experiments on the AMI meeting corpus: 
- python experiment_ami.py hparams/ecapa_tdnn_ami.yaml
  
## License
This project is licensed under the MIT License. The full terms of the MIT License can be found in the LICENSE.md file at the root of this project.

