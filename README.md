# Transformer-Based Drug–Target Affinity Prediction

This project presents a lightweight Transformer-based deep learning model for predicting drug–target binding affinity using raw SMILES strings and protein amino acid sequences. It provides a reproducible pipeline using the Davis dataset to train and evaluate a sequence-based regression model.

---

## 🔬 Overview

- **Goal:** Predict continuous binding affinity scores between drug compounds and protein targets
- **Input:** SMILES + Protein Sequence
- **Model:** Transformer encoder + Regression head
- **Dataset:** Davis dataset (30k drug–target pairs)
- **Metric:** RMSE (Root Mean Square Error)

---

## 🏗️ Architecture

1. Concatenated `SMILES + sequence` input
2. Tokenization using BERT tokenizer (`bert-base-uncased`)
3. Embedding → 2-layer Transformer Encoder
4. Linear → ReLU → Linear → Scalar output

---

## 📊 Results

- **Test RMSE:** 0.832
- Loss curve and top error samples included

---

