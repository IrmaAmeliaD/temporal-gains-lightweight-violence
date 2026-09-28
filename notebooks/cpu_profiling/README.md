# CPU Profiling

This directory contains the controlled CPU profiling procedures used in
the paper.

The main profiling configuration uses:

- seed-0 checkpoints
- batch size 1
- FP32 inference
- two intra-op threads
- one inter-op thread
- 30 warm-up iterations

Latency includes in-memory preprocessing and inference to logits, while
disk I/O, raw-video decoding, and frame extraction are excluded.
