# Native Temporal Input Length

This directory contains the native temporal-input-length experiments
for MobileNetV2 with and without TSM.

The evaluated temporal budgets are:

T = {1, 2, 4, 8}

Unlike the fixed-T redundancy experiments, changing native T changes
the actual number of frames processed by the model and therefore also
changes clip-level computational cost.
