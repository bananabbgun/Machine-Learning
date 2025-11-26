# Advanced Machine Learning & GenAI Projects (ML2025)

This repository collects selected projects I completed in 2025 while taking the
**ML2025** course and self-studying modern **LLMs** and **diffusion models**.

The focus is on understanding and implementing:
- Instruction fine-tuning for LLMs
- Catastrophic forgetting in safety-related tasks
- Knowledge-level model editing and model merging
- Diffusion models and custom concept learning
- Practical ML/GenAI systems such as RAG and simple agents

Each subdirectory is a project-style reorganization of the original course
homeworks, with notebooks and (in some cases) small utilities.

---

## 📂 Project Overview

### LLM Fine-tuning & Behavior

- `llm-sft-alpaca/`  
  Supervised fine-tuning (SFT) of an open-weight LLM on an Alpaca-style
  instruction dataset using **Unsloth** and **TRL**.  
  Focus:
  - Efficient fine-tuning with LoRA-style adapters  
  - Training configuration and stability  
  - Qualitative before/after comparison on instruction-following tasks  

- `llm-safety-forgetting/`  
  Experiments based on **“Fine-tuning leads to forgetting”** on safety-related
  tasks.  
  Focus:
  - How task-specific fine-tuning affects the model’s original safety behavior  
  - Measuring performance trade-offs and signs of catastrophic forgetting  

- `llm-model-editing-memit/`  
  Knowledge-level **model editing** experiments using a MEMIT-style approach.  
  Focus:
  - Editing specific factual associations in the model  
  - Evaluating whether the edit takes effect and how far it generalizes  
  - Checking locality (how much unrelated knowledge is preserved)  

- `llm-model-merging/`  
  **Model merging** between different fine-tuned LLM checkpoints.  
  Focus:
  - Linear / interpolated merging of model weights  
  - Trade-offs between capabilities from each source model  
  - Basic evaluation before and after merging  

---

### Diffusion & Generative Models

- `diffusion-custom-concepts/`  
  Diffusion-based image generation with **custom concept learning** on top of a
  pre-trained model.  
  Focus:
  - Training a diffusion model / adapter on a small set of images  
  - Generating images that follow prompts involving the new concept  
  - Comparing generations before and after customization  

---

### Earlier ML / GenAI Systems

- `Training Transformer/`  
  Experiments on training Transformer models from scratch on downstream tasks,
  with emphasis on optimization and training dynamics.

- `Retrieval Augmented Generation with Agentic System/`  
  A small **Retrieval-Augmented Generation (RAG)** project with simple
  agent-like behavior (multi-step reasoning / tool calls on top of RAG).

- `Understanding Transformer/`  
  Notebooks for understanding the Transformer architecture from first
  principles (embeddings, attention, residual connections, etc.).

- `Machine Learning Engineering Agent/`  
  Prototype of an “ML engineering agent” that assists with parts of the ML
  workflow (e.g., suggesting experiments or organizing results) inside
  notebooks.

> Note: These projects originate from course assignments in ML2025, but the
> structure and documentation here are curated to serve as a portfolio of my
> 2025 ML/GenAI work.

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Environment:** Jupyter Notebook  
- **Libraries / Topics:**  
  - Transformers, LoRA, Unsloth, TRL  
  - Model fine-tuning, forgetting, model editing, model merging  
  - Diffusion models and custom concepts  
  - RAG, simple agents, ML engineering workflows

---

## 📚 Learning Focus

Through these projects, I worked on:

- Going beyond “just using” pre-trained LLMs, and instead studying how they
  change under fine-tuning, editing, merging, and safety constraints.
- Implementing and debugging real ML pipelines in notebooks, including data
  handling, training loops, evaluation, and qualitative analysis.
- Building small but complete GenAI systems (RAG, agents, customized diffusion)
  that connect modeling with practical applications.
