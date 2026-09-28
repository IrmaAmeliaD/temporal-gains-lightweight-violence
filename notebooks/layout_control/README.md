# Repetition-Layout Control

This directory contains the evaluation-only repetition-layout control
for MobileNetV2+TSM at fixed T=8.

The experiment compares grouped and interleaved repetition at K=2 and
K=4 while preserving the same selected temporal observations.

Evaluations are performed using checkpoints trained with three seeds:
0, 42, and 123.
