# Source-Domain Split

This directory contains the saved arrays used during construction of
the fixed source-domain training and validation partition.

## Files

### `trainval_labels.npy`

Binary class labels for the 3,683 samples included in the combined
training-validation pool.

- Class 0: 1,793 samples
- Class 1: 1,890 samples

### `split_indices_trainval.npy`

A permutation of all indices from 0 to 3,682 used to shuffle the
training-validation pool before partitioning.

The permutation contains no duplicated or missing indices.

## Important Note

These files preserve the original split-related arrays used in the
experiments. They do not independently encode the original video
filenames or dataset identities.

The raw and derived video data are not redistributed in this repository.
