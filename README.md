# Temporal Gains in Lightweight Violence Detection under Domain Shift

Official code and reproducibility materials for the paper:

**Temporal Gains in Lightweight Violence Detection under Domain Shift:
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

Experiments are conducted using EfficientFormerV2-S0 and MobileNetV2
with and without lightweight temporal modeling.

## Datasets

### Source datasets

- Hockey Fight
- Movie Fight
- Violent Flows
- AVDV
- SCFD
- RLVS

### Held-out domains

- RWF-2000
- UCF-Crime Fighting
- Bus Violence

The held-out datasets are not used for training, validation,
hyperparameter selection, or domain adaptation.

## Reproducibility Settings

Training seeds:

```text
0, 42, 123
