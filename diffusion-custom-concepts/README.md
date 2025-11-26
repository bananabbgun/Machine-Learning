## Custom Concept Diffusion

This project tailors diffusion models to learn a bespoke visual concept, mixing
off-the-shelf **BLIP Diffusion** inference with a scaffold for custom fine-
tuning runs.

### Components
- GPU + dependency bootstrap plus cloning of the TA starter repo.
- BLIP Diffusion pipeline definition, batched inference over the provided
  metadata, and zipped submission packaging.
- Placeholder training utilities (dataset class, collate fn, trainer launcher)
  ready for experimentation with parameter-efficient fine-tuning.

### Files
- `custom-concept-diffusion.ipynb` – notebook containing the complete workflow
  for inference plus commented templates for full custom diffusion training.
