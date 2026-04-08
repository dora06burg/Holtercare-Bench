# Holtercare-Bench: A Multimodal Benchmark for Evaluating Long-Term Dynamic ECG Analysis

This repository contains the supplementary materials, the complete QA dataset, and data access instructions for the paper **"Holtercare-Bench: A Multimodal Benchmark for Evaluating Long-Term Dynamic ECG Analysis"**. 

## 1. Supplementary Appendix

We provide a supplementary document (`Appendix.pdf`) that contains extended details and results omitted from the main manuscript due to space constraints. The appendix includes:

* **Detailed Distribution of Clinical Annotations:** Exhaustive frequency tables for all beat-level and rhythm-level annotations within Holtercare-23K, demonstrating its clinical scale and diversity.
* **Prompt Templates:** The exact, full-text prompt structures utilized by GPT-5-mini for both the automated HolterAgent QA generation pipeline and the LLM-as-a-judge report evaluation system.
* **Supplemental Experimental Results:** Extended textual generation performance evaluations, including comprehensive BLEU n-gram overlap metrics for both *Open-QA* and *Report Generation* tasks.

## 2. Holtercare-23K QA Dataset

The `QA/` directory contains the complete 22,980 multimodal QA pairs of Holtercare-23K. 

- **Splits:** The data is properly partitioned into `train`, `valid`, and `test` sets at the independent patient case level to prevent data leakage.
- **Task Coverage:** The dataset comprehensively covers the 12 fine-grained sub-tasks across the 3 main cognitive tiers: *Closed-QA*, *Open-QA*, and *Report Generation*.
- **Format:** All files are provided in standard `JSON` format. The construction of these QA pairs is deeply grounded in the de-identified patient information and our robust **tri-level annotation system**.

## 3. Raw ECG Data Access (For Reviewers)

The raw, continuous Holter ECG data corresponding to the Holtercare-23K benchmark is hosted on HuggingFace: **[HuggingFace Link](https://huggingface.co/datasets/Holtercare/Holtercare-23K)**

**Current Status: Private Repository (Pre-publication Embargo)**
Please note that the HuggingFace repository is currently set to **Private**. While the dataset has been rigorously de-identified and fully complies with medical ethics and privacy regulations, it is currently under a pre-publication embargo. This temporary private status ensures that:
1. The data remains secure during the final, routine institutional administrative audit required prior to a permanent open-source public release.
2. We prevent any unauthorized usage or scooping of the dataset before the paper is officially accepted and published.

**Access Instructions & Single-Blind Compliance:**
We are fully committed to allowing reviewers to thoroughly inspect the raw clinical data. However, asking reviewers to request access to a private or gated repository using their personal HuggingFace accounts would reveal their identities to the authors, thereby violating the single-blind review process.

To strictly protect **reviewer anonymity**, we have provided a dedicated, anonymous login account directly to the conference organizers, as per the dataset track guidelines. 

Reviewers who wish to inspect the raw Holter files can obtain this anonymous account from the track chairs. Logging in with this credential will grant immediate access to the private repository without compromising your anonymity.
