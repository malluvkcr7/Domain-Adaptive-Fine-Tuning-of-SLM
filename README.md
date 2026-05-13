# Domain-Adaptive Fine-Tuning of SLM

This repository contains experiments for **domain-adaptive fine-tuning of small language models (SLMs)** across multiple domains, with notebook-based workflows for:

- data preparation and prompt formatting
- parameter-efficient fine-tuning (primarily QLoRA/LoRA)
- domain-specific evaluation

## Repository Purpose

The goal is to study how compact instruction-tuned models can be adapted to specialized domains (medical, finance, and cybersecurity) using domain datasets, then evaluated for task quality and response behavior.

## Repository Structure

- `Medical Domain/`
  - `MedicalFineTuning.ipynb`: medical-domain fine-tuning workflow (dataset preparation, training, and evaluation steps).
  - `trulens_eval.ipynb`: TruLens-based evaluation flow for medical prompts and outputs.

- `finance/`
  - `finance-finetuning.ipynb`: financial-domain fine-tuning experiments across multiple financial tasks/datasets.
  - `trulens_eval.ipynb`: TruLens-based evaluation flow for finance tasks.

- `securityy domain/`
  - `notebook_fixed.ipynb`: cybersecurity multi-task data processing and fine-tuning pipeline.
  - `Dataset Details.xlsx`: dataset reference/details used by the security workflow.

## Notes

- Most workflows are designed for notebook environments such as Kaggle/Colab with GPU support.
- Dependencies are installed inside notebooks.
- The repository currently focuses on experiment notebooks rather than a packaged Python module.
