# CSCR3207 - LLM & Generative AI Mini Projects

This repository contains two mini-project notebooks exploring natural language processing and generation techniques using pretrained embeddings and text datasets.

## Contents

- `Mini Project 1.ipynb` — Notebook for the first mini project (exploratory analysis and models).
- `Mini Project 2.ipynb` — Notebook for the second mini project (experiments with generative models / downstream tasks).
- `resources/` — Folder with datasets and supporting files used by the notebooks:
  - `Articles.csv`
  - `Boston.csv`
  - `financial_news_events.xlsx`
  - `harrypotter.txt`
  - `news_article_labels.csv`
  - `news_articles.csv`
  - `Product_Reviews.csv`
  - `glove.6B/` — pretrained GloVe embeddings (50d, 100d, 200d, 300d)

## Overview

These notebooks are intended for teaching and experimentation with NLP tasks such as:

- Text preprocessing and exploratory data analysis (EDA)
- Word embeddings (GloVe) usage
- Text classification or labeling experiments
- Simple generative modeling or text synthesis experiments

## Setup

1. Create and activate a Python virtual environment (recommended):

```bash
python3 -m venv .venv
source .venv/bin/activate
```

1. Install common data science packages if not already available. The notebooks assume packages such as:

- numpy, pandas
- scikit-learn
- matplotlib or seaborn
- jupyter
- nltk or spacy (optional, for preprocessing)

Install with pip:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter nltk spacy
```

If you plan to use deep learning libraries, also install PyTorch or TensorFlow as needed.

## Usage

1. Start Jupyter Notebook / Lab from the repository root:

```bash
jupyter notebook
```

1. Open `Mini Project 1.ipynb` or `Mini Project 2.ipynb` and run the cells. The notebooks read data from the `resources/` folder; ensure the path is correct if you move files.

## Notes on GloVe embeddings

The `resources/glove.6B/` directory contains pretrained GloVe vectors. Loading the full 300d embeddings may take time and memory — prefer 50d or 100d for quick experiments.

## Suggested Experiments / Next Steps

- Add a `requirements.txt` or `environment.yml` to pin dependencies.
- Convert notebooks to modular Python scripts for repeatable experiments.
- Add small unit tests for preprocessing functions.
- Try fine-tuning a small transformer model on one of the datasets (use Hugging Face Transformers).

