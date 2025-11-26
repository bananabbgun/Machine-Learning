# Fine-tuning Leads to Forgetting (Safety Experiments)

This project studies how fine-tuning an LLM on a math-reasoning task impacts
its original **safety behavior**, following the “fine-tuning leads to
forgetting” hypothesis.

## What this project does
- Fine-tunes `meta-llama/Llama-3.2-1B-Instruct` on GSM8K-like math prompts.
- Evaluates:
  - Downstream accuracy on GSM8K and AILuminate.
  - Changes in the model’s answers to safety-oriented prompts.
- Generates leaderboard-ready prediction files and captures training configs.

## Key ideas
- Task-specific fine-tuning can overwrite general knowledge, including safety.
- There is a measurable trade-off between target-task performance and preserved
  safety behaviors.
- Forgetting is estimated by comparing responses **before vs. after** SFT on a
  reference benchmark.

## Files
- `safety-fine-tuning-forgetting.ipynb` – complete notebook with data download,
  TRL training loop, inference helpers, and export scripts.
