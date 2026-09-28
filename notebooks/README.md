# Fixed-T Temporal Redundancy

This directory contains the fixed-input-length experiments used to
separate the number of physically processed temporal positions (`T`)
from the number of distinct temporal observations (`K`).

Reducing `K` increases temporal redundancy while keeping the nominal
input length and clip-level computational workload fixed.

The evaluated configurations include:

- MobileNetV2
- MobileNetV2+TSM
- EfficientFormerV2-S0 + FrameMean
- EfficientFormerV2-S0 + BiLSTM
- EfficientFormerV2-S0 + TSM + FrameMean

The original notebooks referred to these experiments as
"FrameDiversity"; the public repository uses the terminology
"fixed-T temporal redundancy" to remain consistent with the manuscript.
