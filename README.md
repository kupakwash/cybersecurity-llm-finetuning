📌 Fine-Tuning GPT-4o-mini for Cybersecurity Incident Classification & Solution Generation
🧠 Project Overview

This project demonstrates the domain adaptation of a Large Language Model (LLM) for cybersecurity applications by fine-tuning GPT-4o-mini on a structured incident dataset.

The system is designed to:

Classify cybersecurity incidents based on textual descriptions

Identify attack categories and techniques

Generate concise, actionable remediation steps aligned with Security Operations Center (SOC) workflows

This work explores how lightweight LLMs can be specialized for operational security intelligence without requiring large-scale model retraining.

🎯 Motivation

Modern organizations generate massive volumes of security alerts, logs, and reports.
Manual analysis is:

Time-consuming

Error-prone

Difficult to scale

Generic LLMs lack contextual understanding of cybersecurity terminology.
Fine-tuning enables the model to learn domain-specific semantics and support analysts with faster, more consistent decision-making.

⚙️ Methodology
1️⃣ Data Preparation

Structured cybersecurity dataset containing:

Incident titles / descriptions

Attack categories

MITRE-aligned techniques

Recommended mitigation actions

2️⃣ Instruction–Response Transformation

Each record converted into conversational fine-tuning format:

System → SOC analyst role definition
User → Incident description
Assistant → Classification + recommended solution

3️⃣ Model Fine-Tuning

Base Model: GPT-4o-mini

Supervised fine-tuning using curated cybersecurity samples

Optimized hyperparameters to ensure stable convergence

4️⃣ Evaluation

Performance assessed using:

Classification accuracy trends

BLEU / ROUGE similarity metrics

Qualitative comparison with expert-written solutions

📊 Key Outcomes

Demonstrated strong domain adaptation capability

Generated remediation strategies closely aligned with SOC practices

Achieved high semantic similarity to expert responses

Validated feasibility of using compact LLMs for cybersecurity automation

🛠️ Technology Stack
Component	Tools Used
Language	Python
LLM	GPT-4o-mini
Data Processing	Pandas, NumPy
Development	Jupyter Notebook
Evaluation	BLEU, ROUGE Metrics
Workflow	OpenAI Fine-Tuning Pipeline
📁 Repository Structure
cybersecurity-llm-finetuning/
│
├── notebooks/
│   └── Fine_Tuning_notebook.ipynb
│
├── docs/
│   └── Project_Report.pdf
│
├── README.md
└── requirements.txt
🔐 Environment Setup

Create a .env file locally (do NOT commit it):

OPENAI_API_KEY=your_api_key_here

The notebook reads credentials securely using environment variables.

🚀 Running the Project

Install dependencies:

pip install -r requirements.txt

Launch Jupyter:

jupyter notebook

Execute the fine-tuning workflow inside:

notebooks/Fine_Tuning_notebook.ipynb
🔬 Research Contribution

This project shows that lightweight foundation models can be effectively specialized for cybersecurity reasoning tasks, enabling:

Faster incident triage

AI-assisted threat interpretation

Scalable SOC decision support systems

📈 Future Work

Integration with SIEM platforms for real-time deployment

Multi-turn reasoning for investigation workflows

Explainable AI for analyst trust

Expansion to live threat-intelligence streams

👤 Author

Kupakwashe T. Mapuranga
M.Tech – Artificial Intelligence & Machine Learning
Focus: Applied AI Systems · LLM Fine-Tuning · AI for Security & Sustainability
