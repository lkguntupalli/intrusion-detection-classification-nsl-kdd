# Intrusion Detection Classification Using NSL-KDD

## Overview

This project evaluates and compares three supervised machine learning classification algorithms for intrusion detection using the NSL-KDD dataset:

- Logistic Regression (LR)
- Support Vector Machine with an RBF kernel (SVM)
- Random Forest (RF)

The models are evaluated on both **binary classification** (Normal vs. Attack) and **multiclass classification** (Normal, DoS, Probe, R2L, and U2R). The project also investigates class weighting to address class imbalance and decision-threshold selection for binary classification.

## Repository Structure

```text
intrusion-detection-classification-nsl-kdd/
├── README.md
├── requirements.txt
├── notebooks/
│   ├── 01_binary_classification.ipynb
│   └── 02_official_multiclass_validation.ipynb
└── datasets/
    └── nsl-kdd/
        └── README.md
```

## Dataset

This project uses the [NSL-KDD dataset]](https://www.kaggle.com/datasets/hassan06/nslkdd). The dataset files are included in this repository.

See [`datasets/nsl-kdd/README.md`](datasets/nsl-kdd/README.md) for dataset instructions.

## Setup

1. Clone this repository:

   ```bash
   git clone https://github.com/lkguntupalli/intrusion-detection-classification-nsl-kdd.git
   cd intrusion-detection-classification-nsl-kdd
   ```

2. (Optional) Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   ```

   On Linux/macOS:

   ```bash
   source .venv/bin/activate
   ```

   On Windows:

   ```bat
   .venv\Scripts\activate
   ```

3. Install the required packages:

   ```bash
   python -m pip install -r requirements.txt
   ```

4. Launch Jupyter:

   ```bash
   jupyter notebook
   ```

5. Open and run the notebooks in the `notebooks/` directory.

## Notebooks

| Notebook | Description |
|----------|-------------|
| [`01_binary_classification.ipynb`](notebooks/01_binary_classification.ipynb) | Binary intrusion detection, model comparison, validation-based decision-threshold selection, and evaluation on the official test set. |
| [`02_official_multiclass_validation.ipynb`](notebooks/02_official_multiclass_validation.ipynb) | Multiclass classification, model comparison, and class-weighting experiments using the five attack categories. |

## Evaluation

The models are compared using classification metrics such as accuracy, precision, recall, and F1-score. The experiments also consider confusion matrices, computational cost, and the impact of class imbalance.

## Reproducibility

The notebooks contain the data preprocessing steps, model configurations, and evaluation procedures. Results may vary slightly depending on the software versions and execution environment.

## Authors

- Lakshmikanth Guntupalli ([@lkguntupalli](https://github.com/lkguntupalli))
- Praneeth Reddy Brahmanpally (@PRANEETHREDDY0913)
- sandya kommula (@sandyakommula@gmail.com)  
    

