## MEMIT Model Editing Experiments

This project explores **knowledge-level model editing** using MEMIT/ROME-style
methods on `gpt2-xl`, highlighting how specific factual associations can be
patched without full retraining.

### Highlights
- Colab-friendly setup that clones the MEMIT repo, installs dependencies, and
  loads pretrained checkpoints.
- Utility helpers for grabbing parameters, generating text, printing deltas, and
  scoring locality.
- Two editing paths:
  - **Fine-tuning (FT)** adapters on a small dataset of edits.
  - **ROME/MEMIT** direct weight updates via closed-form math.
- TODO blocks to customize single-edit prompts, multi-edit datasets, and method
  selection.

### Files
- `memit-model-editing.ipynb` – main notebook that configures the environment,
  defines helper functions, and runs the editing + evaluation loops.
