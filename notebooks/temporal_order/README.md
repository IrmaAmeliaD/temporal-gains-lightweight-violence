# Temporal-Order Perturbation

This directory contains inference-time temporal-order perturbation
experiments performed on frozen checkpoints.

The evaluated conditions are:

- Original
- Reverse
- Shuffle-25%
- Shuffle-50%
- Shuffle-100%

Frame identity, frame count, preprocessing, and model parameters are
kept unchanged. FrameMean is included as a permutation-invariant
negative control.

Shuffle conditions use 10 reproducible permutations for each
checkpoint.
