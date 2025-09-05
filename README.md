# Resume Section Classifier (DistilBERT)

This project fine-tunes **DistilBERT** to classify segments of resumes into categories like  
*Education, Skills, Projects, Experience, Certifications, etc.*  

It complements the **Resume Segmenter (LLM Pipeline)** by training a lightweight transformer model for fast inference.

---

## 📌 Project Overview
- **Input Dataset**: Created from structured JSON resumes.
  - `train.jsonl` (3024 samples)
  - `val.jsonl` (757 samples)
- **Model**: DistilBERT (`distilbert-base-uncased`) with classification head.
- **Training Setup**:
  - 5 epochs
  - Batch size = 8
  - Optimizer = AdamW
  - Metrics = Accuracy & Weighted F1

---

## 📊 Results
- **Validation Accuracy**: ~98.0%
- **Weighted F1 Score**: ~97.9%
- **Training Time**: ~6 hours on GPU

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
- LLMs are powerful but costly for inference.
- DistilBERT offers **fast, efficient classification** suitable for deployment.
- Demonstrates ability to fine-tune state-of-the-art NLP models.

---

## 🧠 Skills Demonstrated
- Dataset engineering (`train.jsonl`, `val.jsonl`).
- Transformer fine-tuning with Hugging Face.
- Model evaluation (accuracy, F1).
- Saving & exporting models for deployment.
