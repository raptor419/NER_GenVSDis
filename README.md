# Comparing Basic Generative and Discriminative Approaches for Named Entity Recognition

## Introduction
In this project, we do a comparative analysis of the performance of very basic Generative Models namely Hidden Markov Models (HMMs), and Discriminative Models namely Bidirectional Long Short-Term Memory (BiLSTM) Neural Networks in a Named Entity Recognition (NER) problem statement on the CoNLL dataset.

## Requirements

### Dependencies
```
jupyter
nltk
numpy
pandas
spacy
tqdm
sklearn
keras
tensorflow
matplotlib
seaborn
```

### System Requirements
GPU with Tensorflow backend support for keras
GPU and RAM enough to load and process Glove Embeddings

### Google Colab Alternative
Can also be run exclusively on Google Colab on the following notebook: https://colab.research.google.com/drive/11eRt4IHMlJX3KfTlR2UjW0ED59AuHAMI

## Steps to run
### Locally
```
pip install jupyter nltk numpy pandas spacy tqdm sklearn keras tensorflow matplotlib seaborn
jupyter notebook
```
Open `NLP Project Final Code.ipynb` in Jupyter.

### Colab
Colab notebook https://colab.research.google.com/drive/11eRt4IHMlJX3KfTlR2UjW0ED59AuHAMI should run natviely without any setup.

## Summary
The With Hidden Markov Model and BiLSTM Model perform 0.83 and 0.67 macro average F1-Score. We also generate synthetic data using the trained HMM generative model. For synthetic data Hidden Markov Model and BiLSTM Model perform 0.64 and 0.26 macro average F1-Score. Both approaches perform worse on synthetic data vs real data when trained on the same set, but that is most likely due to inaccurate data generation by the HMM Model.
 
In general, though the BiLSTM is more complex than the HMMs, even considering the synthetic data analysis, but doesn’t necessarily produce higher prediction accuracy than HMM. While both approaches have their own advantages and disadvantages. The discriminative approach seems to be a better approach for a balanced dataset while the generative approach seems better for an unbalanced dataset for the named entity recognition problem.
