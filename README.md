# Holtercare-Bench: A Multimodal Benchmark for Evaluating Long-Term Dynamic ECG Analysis

This repository contains the complete QA dataset for the paper **"Holtercare-Bench: A Multimodal Benchmark for Evaluating Long-Term Dynamic ECG Analysis"**. The `QA/` directory contains the complete 22,980 multimodal QA pairs of Holtercare-23K. 

- **Splits:** The data is properly partitioned into `train`, `valid`, and `test` sets at the independent patient case level to prevent data leakage.
- **Task Coverage:** The dataset comprehensively covers the 12 fine-grained sub-tasks across the 3 main cognitive tiers: *Closed-QA*, *Open-QA*, and *Report Generation*.
- **Format:** All files are provided in standard `JSON` format. The construction of these QA pairs is deeply grounded in the de-identified patient information and our robust **tri-level annotation system**.
