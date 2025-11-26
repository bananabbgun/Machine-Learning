## Alpaca Instruction SFT with Unsloth

This project walks through a lightweight yet production-style instruction
fine-tuning pipeline for open-weight LLMs using **Unsloth** + **TRL** on the
Alpaca/ShareGPT conversations.

### What’s inside
- GPU / dependency bootstrap that mirrors a real Colab or Kaggle workflow.
- Data-engineering steps to **sort** and **filter** 52k Alpaca-style examples,
  with both simple (length-based) and advanced (length + score) heuristics.
- LoRA configuration using `FastLanguageModel.get_peft_model`, exposing ranks,
  adapter targets, dropout, and gradient checkpointing tweaks.
- Training orchestration via `SFTTrainer`, response-only loss masking, optional
  curriculum training, and qualitative inference helpers.
- Saving / loading adapters locally for rapid iteration.

### Files
- `alpaca-unsloth-sft.ipynb` – end-to-end notebook covering setup, data prep,
  training, inference, and export steps.
