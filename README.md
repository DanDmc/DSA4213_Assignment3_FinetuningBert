# Assignment 3: Fine-tuning FinBERT with LoRA for Financial Sentiment Classification

**Author:** Daniel Christopher Chan (A0253408H)  
**Course:** DSA4213 — Natural Language Processing  

---

## 🧠 Overview
This repository contains the code and report for **Assignment 3: Fine-tuning Pretrained Transformers**.  
The goal is to evaluate and compare **FinBERT** and **BERT-base** for financial sentiment classification on the **Financial PhraseBank** dataset, using both **full fine-tuning** and **Low-Rank Adaptation (LoRA)** (for FinBERT).

---

## 🚀 Running the Notebook

### Option 1: Google Colab (recommended)
1. Open the notebook in Colab:
   - [Open in Colab]([https://colab.research.google.com/github/DanDmc/DSA4213_Assignment3_FinetuningBert/blob/main/DSA4213_Assignment3_A0253408H_Code.ipynb))
2. In Colab:
   - Go to **Runtime → Change runtime type → GPU (T4 preferred)**.
   - Run all cells sequentially.
3. The notebook will:
   - Clone this repo and get the Financial PhraseBank dataset that has been downloaded from https://huggingface.co/datasets/takala/financial_phrasebank
   - Fine-tune BERT and FinBERT using both **full fine-tuning** and **LoRA (r=4,8,16)**.
   - Output evaluation metrics, confusion matrices, efficiency summaries, and error analysis.

### Option 2: Local execution (optional)
If you prefer running locally (GPU may be required):
```bash
pip install -r requirements.txt
jupyter notebook finetune_finbert_lora.ipynb
