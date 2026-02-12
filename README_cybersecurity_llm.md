# Fine-Tuning GPT-4o-mini for Cybersecurity Incident Classification and Solution Generation

## Overview

This project fine-tunes GPT-4o-mini on a structured cybersecurity
dataset to classify incidents and generate actionable remediation steps.
It demonstrates domain adaptation of a lightweight LLM for Security
Operations Center (SOC) support.

## Motivation

Security teams process massive volumes of alerts and reports. Manual
analysis is slow and inconsistent. This research investigates whether
supervised fine-tuning can enable an LLM to understand cybersecurity
terminology and recommend accurate solutions automatically.

## Methodology

1.  Data Cleaning and Validation (CSV dataset)
2.  Conversion to Instruction--Response JSONL format
3.  Supervised Fine-Tuning of GPT-4o-mini
4.  Evaluation using BLEU, ROUGE, Accuracy, and Loss trends

## Results

-   Accuracy stabilized around \~81% during evaluation.
-   BLEU score ≈ 0.90 indicating strong semantic similarity to expert
    solutions.
-   Training showed stable convergence without overfitting.

## Tech Stack

Python • Pandas • NumPy • Jupyter • OpenAI Fine-Tuning API • NLP
Evaluation Metrics

## Repository Structure

cybersecurity-llm-finetuning/ ├── notebooks/ ├── docs/ ├── README.md └──
requirements.txt

## Dataset Note

Dataset not included due to size/privacy. Use a structured cybersecurity
incident dataset with fields such as Incident Title, Category,
Technique, and Solution.

## Future Work

Integration with SIEM tools, real-time SOC deployment, explainable AI,
and multi-turn reasoning.

## Author

Kupakwashe T. Mapuranga M.Tech AI & ML --- Applied LLM Systems &
Cybersecurity AI
