# Results

This folder contains processed numerical results corresponding to the tables and figures reported in the paper.
# Experimental Results

This directory contains the processed numerical results used to
construct the tables and figures reported in the manuscript.

Where applicable, results are provided at the individual training-seed
level (`0`, `42`, and `123`) rather than only as aggregated
mean ± standard deviation.

The files correspond to the main experimental analyses:

- `overall_performance.csv`: main model comparison
- `native_T_results.csv`: native temporal input length
- `fixed_T_efficientformer.csv`: EfficientFormerV2 fixed-T redundancy
- `fixed_T_mobilenet.csv`: MobileNetV2 fixed-T redundancy
- `matched_Ktrain4_results.csv`: matched train-time redundancy control
- `layout_control_results.csv`: grouped-versus-interleaved control
- `aggregation_consistency.csv`: seed-wise temporal aggregation analysis
- `temporal_order_results.csv`: temporal-order perturbations
- `temporal_order_prediction_diagnostics.csv`: prediction-level order diagnostics
- `paired_bootstrap_results.csv`: paired stratified bootstrap analysis
- `cpu_mobilenet.csv`: MobileNetV2 computational profiling
- `cpu_efficientformer.csv`: EfficientFormerV2 computational profiling

Raw video datasets are not distributed with this repository.
