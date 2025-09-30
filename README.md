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
  
Similarly, use the corresponding files for **DIHARD-III** and **VoxConverse**.

## Instructions for implementation
## Instructions
Our implementation is based on a modified version of the AMI recipe in SpeechBrain.  
To launch an experiment (example: AMI meeting corpus), run the following command from the directory where your `experiment_ami.py` file is located:

```bash
python experiment_ami.py hparams/ecapa_tdnn_ami.yaml
```  
## License
This project is licensed under the MIT License. The full terms of the MIT License can be found in the LICENSE.md file at the root of this project.

