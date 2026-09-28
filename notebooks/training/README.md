# Matched Ktrain=4 Training

This directory contains the training notebooks used to generate the
MobileNetV2+TSM checkpoints for the matched train-time redundancy control.

The purpose of this experiment is to distinguish sensitivity to reduced
temporal diversity from train-test redundancy mismatch.

## Experimental Setting

The physical temporal input length is fixed at:

T = 8

while the number of distinct temporal observations used during training is:
Ktrain = 4

Two repetition layouts are evaluated:
Grouped repetition
[A, A, B, B, C, C, D, D]

Interleaved repetition
[A, B, C, D, A, B, C, D]

Both layouts contain the same four distinct temporal observations but
present different local adjacency structures to the Temporal Shift Module
(TSM).
Training Seeds
Checkpoints are trained independently using:
0, 42, 123

The dataset split is kept fixed using:
FIXED_SPLIT_SEED = 42

Thus, cross-seed variation reflects training stochasticity rather than
changes in train-validation-test composition.
Expected Checkpoints
The training notebooks generate checkpoints for:
MobileNetV2+TSM
T = 8
Ktrain = 4

under:
grouped repetition
interleaved repetition

These checkpoints are subsequently evaluated using the fixed-T redundancy
and repetition-layout control experiments.
Relation to the Paper
These checkpoints support the matched train-time redundancy analysis and
the grouped-versus-interleaved adjacency control reported in the manuscript.
The corresponding evaluation notebooks are located in:
notebooks/fixed_T_redundancy/
notebooks/layout_control/
