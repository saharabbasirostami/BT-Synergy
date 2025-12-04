# BT-Synergy

**BT-Synergy** is a deep learning framework for predicting drug synergy, built on a **Transformer enhanced with BiLSTM** architecture.  

## Key Features

- **Drug representation using SELFIES** for molecular sequence feature extraction.  
- **Pre-trained protein embeddings** for cellular and protein feature representation.  
- **Attention Pooling** for intelligent aggregation of protein embeddings.  
- **Simple Dual Fusion** for combining drug and cell features.  
- **Quartile-based labeling** to handle class imbalance in synergy data.

## Code Structure

- `setup.py`: Installs dependencies and sets up Google Colab environment.  
- `data_utils.py`: Loads data, constructs drug-protein and protein-cell matrices, applies Attention Pooling.  
- `main.py`: Defines model, training, 5-fold cross-validation, and external test evaluation.

## Datasets

- **DrugCombDB** and **OncologyScreen** for drug and cell line data.  
- Input files: `drug_protein.csv`, `cell_protein.csv`, `drug_combinations.csv`.

## Training & Evaluation

- K-Fold Cross Validation (5-fold) with 10% external test set.  
- Final model saved in H5 format.

## Quick Install

```bash
pip install -r requirements.txt
