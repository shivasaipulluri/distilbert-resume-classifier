# DistilBERT Resume Classification (Applied Research @ Lucerna Labs)

This applied research project fine-tuned **DistilBERT** to classify resume sections  
into categories like *Education, Skills, Projects, Experience, Achievements, etc.*  

---

## 📌 Project Overview
- **Dataset**: ~3,000 training samples, ~750 validation samples.
- **Model**: DistilBERT (`distilbert-base-uncased`) with classification head.
- **Training Setup**:
  - 5 epochs
  - Batch size = 8
  - Optimizer = AdamW
  - Runtime = ~6 hours
- **Evaluation Metrics**:
  - Accuracy
  - Weighted F1 score

---

## 📊 Results
- **Training Loss**: ~0.1256
- **Validation Loss**: ~0.1273
- **Validation Accuracy**: ~98.0%
- **Weighted F1 Score**: ~97.9%

---

## 📂 Repository Structure
distilbert-resume-classifier/
├── prepare_dataset.ipynb # JSON → train/val dataset
├── train_resume_model.ipynb # Training notebook
├── Distilbert_model.ipynb # Final model training & evaluation
├── train.jsonl # Training dataset
├── val.jsonl # Validation dataset
├── resume-segmenter/ # Saved model & tokenizer
└── README.md

---

## 🚀 Why This Project
- Addresses **resume parsing automation** for HR tech.
- Shows ability to **fine-tune and evaluate transformers**.
- Research-grade experiment with high accuracy results.
- LLMs are powerful but costly for inference.
- DistilBERT offers **fast, efficient classification** suitable for deployment.
- Demonstrates ability to fine-tune state-of-the-art NLP models.

---

## 🧠 Skills Demonstrated
- Dataset engineering (`train.jsonl`, `val.jsonl`).
- Transformer fine-tuning with Hugging Face.
- Model evaluation (accuracy, F1).
- Saving & exporting models for deployment.
- Hugging Face Trainer API.
- Transformer fine-tuning (DistilBERT).
- Model evaluation (accuracy, F1).
- Building end-to-end inference pipeline.
