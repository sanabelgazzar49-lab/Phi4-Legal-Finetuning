# Phi4-Legal-Finetuning
"Fine-tuning Phi-4 for specialized legal reasoning using the SCOTUS 2024 dataset. This project utilizes LoRA adapters and Unsloth to enhance model precision and recall in judicial analysis, achieving a 42% improvement in F1-score. Deployment-ready via Ollama and GGUF."
LegalPhi: Fine-Tuning Phi-4 for Enhanced Judicial ReasoningLegalPhi is an AI-driven project focused on specialized Natural Language Processing (NLP) within the legal domain.
By fine-tuning Microsoft’s Phi-4 (a small language model) on the SCOTUS 2024 decisions dataset, this project aims to bridge the gap between general-purpose AI and precise judicial reasoning.
🚀 Project OverviewModel:
Phi-4.Task: Judicial Reasoning & Legal Analysis.
Dataset: SCOTUS 2024 Decisions (relai-ai/legal-scenarios-SCOTUS-2024-decisions).
Technique: Parameter-Efficient Fine-Tuning (PEFT) using LoRA via the Unsloth library.
📊 Evaluation Results
The model was evaluated using the F1-Score to measure the balance between Precision and Recall. 
The fine-tuning process demonstrated a significant improvement in capturing complex legal patterns.
Model ArchitectureAverage F1-ScoreRelative ImprovementPhi-4 (Baseline)11.84%-LegalPhi (Fine-Tuned)16.89%+42.65%Key 
Metrics Explained:Precision: Reflects the accuracy of the legal terminology used by the model.
Recall: Measures the model's ability to cover and retrieve essential legal reasoning from the ground truth.
F1-Score: Shows a consistent 42% boost, proving the effectiveness of domain-specific training.
🛠️ Deployment with OllamaTo ensure data privacy and accessibility, the model is optimized for local deployment.
Merging: LoRA weights were merged with the base model for a standalone architecture.
Quantization: Converted to GGUF (4-bit) to run efficiently on standard consumer hardware.
Local Execution: Fully operational via Ollama using a custom Modelfile for consistent prompt templating.
💻 Tech StackFrameworks: Hugging Face, Unsloth, PEFT.Infrastructure: Google Colab Pro (A100 GPU).Deployment: Ollama, GGUF.
