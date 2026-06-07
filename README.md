# NLP Recipes and Text ML

Applied NLP notebooks covering sentiment analysis, summarization, classification, information retrieval, and sequence modeling. Adapted from *Natural Language Processing Recipes* (Kulkarni and Shivananda) with custom extensions.

## Problem

Demonstrate end-to-end NLP workflows from raw text to deployed models across common business use cases.

## Approach

| Notebook | Use case |
|----------|----------|
| Sentiment Analysis.ipynb | Polarity classification |
| Summarizing the data - TextRank.ipynb | Extractive summarization |
| Resume matching .ipynb | Semantic job-resume matching |
| Predicting next Word LSTM .ipynb | Language modeling |
| chat generator.ipynb | Conversational text generation |
| Clustering Documents.ipynb | Unsupervised topic grouping |
| Classification using Neural Network.ipynb | Multi-class text classification |
| Text Similarity.ipynb | Embedding-based similarity |

## Reproducibility

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

Download NLTK corpora if needed:

```python
import nltk
nltk.download("punkt")
nltk.download("stopwords")
```

## Tech stack

Python 3, Jupyter, NLTK, scikit-learn, TensorFlow/PyTorch (notebook-specific)

## Overlap note

Several notebooks mirror [Personal-Projects](https://github.com/baban9/Personal-Projects). Treat this repo as the NLP-focused index; Personal-Projects covers broader ML domains.

## Limitations and next steps

- Extract shared preprocessing into a `nlp_utils/` package
- Add pytest smoke tests for each notebook's import cells
- Consolidate duplicate notebooks into one canonical repo

## Reference

Kulkarni, A. and Shivananda, A. *Natural Language Processing Recipes*. Packt Publishing.
