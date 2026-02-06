# AMPBAN

This repository contains the source datasets and  code for the paper AMPBAN: A Deep Learning Framework Integrating Protein Sequence and Structural Features for Antimicrobial Peptide Prediction. [bioRxiv](https://www.biorxiv.org/content/10.64898/2026.01.20.700468v1)

---

# Table of contents

1. Installation

2. Datasets and model

3. Example usage

4. Citation

---

## Installation

The model was trained and evaluated with a single `NVIDIA` GeForce RTX 3090 GPU (24 GB VRAM), The software environment adopts python 3.10 and the framework PyTorch 2.5.1 (CUDA 12.4).

You can install it with conda

`conda env create -f environment.yml`





## Datasets and model

The source raw training data can be find in `./data/`

The positive data:

`./data/peptipedia/activities_canon_AMP-20241204.csv`

The negative data:

`./data/Swiss-Prot/uniprotkb_reviewed_true_AND_length_5_TO_2024_12_26.fasta`

The detailed data pre-process and feature extraction program can be find in `AMPBAM_workflow.ipynb`



## Example usage

In this work we meticulously re-implemented four advanced AMP prediction models—AMPScanner, AMPlify, Macrel, and AMP-CLIP—by strictly adhering to the original data processing protocols, feature extraction strategies, and model architectures described in the respective source papers. The related code can be find in:`./5-fold-CV/`

The source 5-cv training code of ampban can be find in `./5-fold-CV/ampban/ampban_cv.ipynb`

here, if you'd like to train a new model with ampban, you can use your training dataset and run it again aftere the feature extraction.



## Citation

AMPBAN: A Deep Learning Framework Integrating Protein Sequence and Structural Features for Antimicrobial Peptide Prediction

Wenhui Bai, Wenhao Yang, Yao-Qing Chen, Hongchao Ji, Lorraine Brennan, Li Wang

bioRxiv 2026.01.20.700468; doi: https://doi.org/10.64898/2026.01.20.700468


