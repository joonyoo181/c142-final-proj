# 5-Fold Cross-Validation of an ANI-Inspired Neural Network on the ANI-1 Dataset

## Overview

This repository showcases a neural network trained on the ANI-1 dataset following the ANI architecture from [this paper](https://pubs.rsc.org/en/content/articlelanding/2017/sc/c6sc05720a), as a submission to UC Berkeley's BIOENG C142 final project.

## Repository Structure

```bash
root/
│
├── dataset/                             # Contains data resources used in the project
│   ├── ani_gdb_s01_to_s04.h5            # ANI-1 dataset (HDF5 format), used for training and evaluation
│   └── paper/
│       └── ANI.pdf                      # Original ANI paper for reference and citation
│
├── trained_models/                      # Saved PyTorch model checkpoints from 5-fold cross-validation
│   ├── ani_model_fold_1.pt              # Trained model from Fold 1
│   ├── ani_model_fold_2.pt              # Trained model from Fold 2
│   ├── ani_model_fold_3.pt              # Trained model from Fold 3
│   ├── ani_model_fold_4.pt              # Trained model from Fold 4
│   └── ani_model_fold_5.pt              # Trained model from Fold 5
│
└── ANI_final.ipynb                      # Final Jupyter notebook containing data loading, model training, evaluation, and visualization
```

## Dependencies

- Python 3.8+
- PyTorch
- TorchANI
- NumPy
- Matplotlib
- tqdm
- pandas

## How to Run

1. Clone this repository.
2. Open `ANI_final.ipynb` in Jupyter Notebook or VSCode.
3. Run all cells to preprocess data, train the model across 5 folds, evaluate, and visualize performance.

