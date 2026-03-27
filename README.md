# Neural Network Capacity, Imbalance, and Generalisation

This repository contains a full tutorial project:

**How Neural Network Capacity and Class Imbalance Affect Generalisation: An Empirical Study on Credit Card Fraud Detection**

It is designed to satisfy course requirements with:
- a web tutorial (`tutorial.html`, <2000 words),
- a reproducible notebook (`fraud_capacity_tutorial.ipynb`),
- references, license, and runnable code.

## Dataset

Place Kaggle `creditcard.csv` in the repository root:

- `creditcard.csv`

Dataset source:
[Kaggle Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## Run Instructions

```bash
pip install -r requirements.txt
python -m jupyter nbconvert --to notebook --execute fraud_capacity_tutorial.ipynb --inplace --ExecutePreprocessor.timeout=1800
```

After execution:
- figures are saved in `figures/`
- `tutorial.html` displays the generated figures.

## What is investigated

- MLP capacity (width and depth)
- Class imbalance handling:
  - baseline (no balancing)
  - class-weighted training via sample weights
  - random undersampling
- Generalisation gap
- Decision-threshold sensitivity analysis (precision/recall/F1 vs threshold)
- Multi-seed robustness analysis (mean ± std)
- Metrics suited for extreme imbalance:
  - Precision
  - Recall
  - F1
  - PR-AUC (Average Precision)

## Accessibility

- Semantic HTML structure with headings and landmarks
- Alt text on all figures
- High-contrast, color-blind-friendly plot palette
- Non-color visual encodings (markers/line styles)
- Reduced-motion support in webpage

## GitHub link reminder

Before submission, replace placeholder URLs in:
- `README.md`
- `tutorial.html`
- any PDF export (if you export one)

Repository placeholder:
`https://github.com/YOUR_USERNAME/YOUR_REPO_NAME`

## References

- Pedregosa et al. (2011), *Scikit-learn: Machine Learning in Python*, JMLR.
- Goodfellow, Bengio, Courville (2016), *Deep Learning*, MIT Press.
- Kaggle dataset page and cited fraud-detection works by Dal Pozzolo et al.
