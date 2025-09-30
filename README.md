# MK-SGC-SC: Multiple Kernel Guided Sparse Graph Construction in Spectral Clustering for Unsupervised Speaker Diarization

### About
This repository contains the implementation for the paper:  
- Nikhil Raghav, Avisek Gupta, Swagatam Das, and Md Sahidullah, *MK-SGC-SC: Multiple Kernel Guided Sparse Graph Construction in Spectral Clustering for Unsupervised Speaker Diarization*, communicated to ICASSP 2026.

## Instructions

Follow the steps below to run the experiments with MK-SGC-SC:

### 1. Install dependencies
- Install SpeechBrain version `0.5.14`.  
- Follow the installation guide in the [SpeechBrain repository](https://github.com/speechbrain/speechbrain).

### 2. Replace files
- Depending on the dataset (**DIHARD-III**, **AMI**, or **VoxConverse**), replace the corresponding files in SpeechBrain with the versions provided in this repository.  
- For example, for the **AMI meeting corpus**, update the files as shown:

| Original file (SpeechBrain)                              | Replace with (from this repo)       |
|----------------------------------------------------------|-------------------------------------|
| `speechbrain/recipes/AMI/Diarization/experiment.py`      | `experiment_ami.py`                 |
| `speechbrain/recipes/AMI/Diarization/hparams/ecapa_tdnn.yaml` | `ecapa_tdnn_ami.yaml`               |
| `speechbrain/speechbrain/processing/diarization.py`      | `diarization_ami.py`                |

### 3. Run the experiment
- Navigate to the directory where your modified `experiment_ami.py` is located.  
- Launch the experiment with the following command:

```bash
python experiment_ami.py hparams/ecapa_tdnn_ami.yaml
```  
## License
This project is licensed under the MIT License. The full terms of the MIT License can be found in the LICENSE.md file at the root of this project.

