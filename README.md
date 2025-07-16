# DRUG-ANALYSIS
Deep learning for drug-target affinity prediction using Davis dataset; cross-evaluated on KIBA.

# Drug-Target Affinity Prediction using Deep Learning (Davis → KIBA)

This project presents a deep learning-based model for predicting drug-target binding affinities. It is trained on the Davis dataset and evaluated on the KIBA dataset using the Therapeutics Data Commons (TDC) framework. The model uses SMILES and protein sequences as inputs, with feature extraction via CNN and multi-head attention mechanisms.

---

## Key Features
- Dataset loading and cleaning using PyTDC
- Tokenization and padding of SMILES and protein sequences
- Custom architecture combining:
  - CNN for SMILES (drug input)
  - Multi-head Attention for protein sequences
  - Weighted feature fusion using Dense layers
- Evaluation on both training (Davis) and external (KIBA) dataset
- Visualization of training curves and prediction scatter plots

---

## Files
- `dti_prediction_davis_kiba.ipynb` – Full notebook with training, evaluation, and visualization
- `README.md` – Documentation and overview of the project

---

## Installation
If running locally (not on Colab), install the required packages:

```bash
pip install PyTDC tensorflow matplotlib scikit-learn pandas
