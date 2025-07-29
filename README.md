# 🔥 BDIFF Forest Fire Classification - Algorithme.ai (XAI - BlackSwan) 

This project leverages the public French dataset **BDIFF** (`Base de Données des Incendies de Forêts en France`) covering forest fires from **2022 to 2025**. Our aim is to **predict whether a fire was of malign origin** (`malveillant`) using modern AI techniques.

## 📦 Repository Structure

```
BDIFF/
├── algorithmeai/
│   ├── BDIFF.py                # Main script for classification
│   ├── automl.py               # AutoML comparisons
│   ├── plot_model.py           # Model plotting and evaluation
│   └── prep-maker.py           # Data preprocessing pipeline
├── data/
│   ├── Dataset-Malveillant-BDIFF.csv  # Raw dataset
│   ├── training.csv                   # Training split
│   └── backtest.csv                   # Backtesting split
├── results/
│   ├── BDIFF_algo-rf-gb.csv           # Model predictions (BlackSwan vs RF/GB)
│   └── BDIFF_algo-rf-gb_performance_auc.pdf  # AUC performance chart
```

## 🔍 Dataset

- **Source**: [BDIFF - Incendies de forêts en France](https://bdiff.agriculture.gouv.fr/incendies)
- **Years**: 2022–2025
- **Target Feature**: `Nature` field (to determine whether a fire was "malveillant")

## 🧠 AI Models

We compared the performance of several algorithms to determine the malign origin of fires:

- 🦢 **BlackSwan** (proprietary model)
- 🌲 Random Forest
- ⚡ Gradient Boosting

All models were benchmarked on the same data splits, and the results are saved in the `results/` folder.

## 🤖 Explainability with RAG

We enhanced interpretability using a **RAG (Retrieval-Augmented Generation)** system. This allows contextual understanding of **why** a fire might be deemed malveillant, drawing on structured features and BlackSwan's ranking mechanism.

## 🚀 Getting Started

### Requirements

- Python 3.8+
- pandas
- scikit-learn
- matplotlib

### Run the main classifier

```bash
cd BDIFF/algorithmeai
python BDIFF.py
```

## 📜 License

This project is released under the **MIT License**. See `LICENSE` for details.

---

© 2025 Algorithme.ai — Make Ai Trustworthy.
