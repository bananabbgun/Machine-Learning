## PEFT-Based LLM Model Merging

This project investigates how to merge multiple LoRA adapters into a single
model, combining capabilities from different tasks (e.g., GSM8K vs. ARC) using
advanced PEFT utilities.

### What you can do here
- Spin up a Colab/Kaggle-like environment, install the TA-provided PEFT fork,
  and download evaluation datasets.
- Configure deterministic seeds, prompt templates, and merge hyperparameters
  (weights, density, majority-sign rules, etc.).
- Run inference pipelines for math (GSM8K) and science (ARC) tasks and export
  Judgeboi-compatible submissions.
- Experiment with multiple merge strategies: linear, TIES, DARE, magnitude
  pruning, and a custom **SCE** algorithm.

### Files
- `peft-model-merging.ipynb` – orchestration notebook that walks through setup,
  merging, evaluation, and packaging submissions.
- `lora_tuner_merge_patch.py` – extensions to `peft.utils.merge_utils` introducing
  higher-level merge algorithms (including SCE).
- `merge_utils_extensions.py` – patched PEFT tuner that wires the new merge modes into
  `LoraModel`.
