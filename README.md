# DistilBERT-Compression-Benchmark
Empirical benchmark evaluating parameter footprint, inference latency, and accuracy retention of DistilBERT against BERT-base.
Empirical Evaluation of DistilBERT Knowledge Distillation vs. BERT-base

This repository contains an experimental benchmark evaluating the model compression and inference latency trade-offs introduced in the DistilBERT paper (Sanh et al., 2019). 

Distillation allows a smaller student model to approximate the behavior of a larger teacher model during pre-training. In this study, I measured parameter size, per-sample inference latency, and classification accuracy between bert-base-uncased and distilbert-base-uncased on a curated text evaluation benchmark.

Experimental Findings

- Parameter Reduction: DistilBERT reduced the total parameter footprint significantly while retaining competitive language understanding capabilities.
- Latency Improvement: Measured inference latency showed marked speedups per sample compared to the full BERT baseline.

Reference

- Sanh, V., Debut, L., Chaumond, J., & Wolf, T. (2019). DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter. arXiv preprint arXiv:1910.01108.

Files

- DistilBERT_Ablation_Study.ipynb - Colab notebook containing model loading, latency profiling, and benchmark visualization.
- distilbert_benchmark_results.png - Output charts comparing parameter size and inference latency.
