# DNABERT-2 embeddings identify glycosyl hydrolase specificity from genomic sequence

This repository contains code and data supporting the manuscript submitted to *Bioinformatics*.

## Overview
We demonstrate that DNABERT-2 sequence embeddings can distinguish functionally specific glycosyl hydrolases from closely related enzymes within a single bacterial genome (*Levilactobacillus brevis* KB290).

## Repository contents
- `01_generate_embeddings.ipynb`: Generates 768-dimensional DNABERT-2 embeddings from DNA sequences
- `02_evaluation_analysis.ipynb`: Performs PCA/UMAP visualization, cosine similarity analysis, and leave-one-out ranking
- `data/posneg_sequences.csv`: Curated positive and hard-negative gene sequences
- `results/`: Output figures used in the manuscript (Figure 2)

## Reproducibility
To reproduce the main results:

1. Install dependencies
```bash
pip install -r requirements.txt

jupyter notebook 01_generate_embeddings.ipynb

jupyter notebook 02_evaluation_analysis.ipynb


---

## 🔹 Step 3-4. requirements.txt (이것도 복붙)

```txt
torch
transformers
numpy
pandas
scikit-learn
matplotlib
seaborn
umap-learn
tqdm
