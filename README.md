# Temporal Gains in Lightweight Violence Detection

Official code and reproducibility materials for the paper:

**Temporal Gains in Lightweight Violence Detection:
Frame Budget, Temporal Interaction and Ordering**

## Overview

This repository contains the code, experimental protocols, evaluation
manifests, and processed results used to investigate temporal information
in lightweight video violence recognition.

The study examines four related temporal factors:

1. processed-frame budget (`T`);
2. number of distinct temporal observations (`K`) at fixed input length;
3. local inter-frame interaction and repetition-induced adjacency;
4. sensitivity to global chronological ordering.

Experiments are conducted using EfficientFormerV2-S0 and MobileNetV2,
with and without lightweight temporal modeling.

## Experimental Setting

### Source datasets

The source-domain experiments use:

- Hockey Fight (HF)
- Movie Fight (MF)
- Violent Flows (VCF)
- Automatic Violence Detection in Videos (AVDV)
- Surveillance Camera Fight Dataset (SCFD)
- Real-Life Violence Situations (RLVS)

### Held-out domains

Cross-domain evaluation is performed on:

- RWF-2000
- UCF-Crime Fighting
- Bus Violence

The held-out datasets are not used for training, validation,
hyperparameter selection, or domain adaptation.

## Reproducibility Settings

Training seeds: 0, 42, 123

Fixed data split seed:42

MobileNetV2 native temporal budgets:T = {1, 2, 4, 8}
At fixed input length, T denotes the number of temporal positions processed by the model, while K <= T denotes the number of distinct temporal observations represented in the sequence.

## Repository Structure

notebooks/
    Training, evaluation, temporal diagnostics, and profiling notebooks

data/
    Dataset manifests and split information

results/
    Processed numerical results reported in the manuscript

## Main Experiments
The repository contains reproducibility materials for:
- native temporal input length;
- fixed-T temporal redundancy;
- grouped-versus-interleaved repetition controls;
- temporal-order perturbation;
- paired bootstrap analysis;
- CPU profiling.
## **Data Availability**
Raw video datasets are not redistributed in this repository.
Users should obtain the datasets from their original sources.
Dataset identifiers and evaluation manifests used in the experiments
will be provided under data/manifests/.
## **Results**
Processed numerical results corresponding to the manuscript tables and
figures will be provided under results/.

## **Citation**
If you use this repository, please cite:
Irma Amelia Dewi et al.
Temporal Gains in Lightweight Violence Detection under Domain Shift:
Frame Budget, Temporal Interaction and Ordering.
