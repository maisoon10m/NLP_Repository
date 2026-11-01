# Lab 11: Attention with RNN

## Description
This lab explores how **Attention Mechanisms** work with **Recurrent Neural Networks (RNNs)** to process natural language questions.

The lab uses PyTorch to build and train an RNN-based model with attention, allowing us to visualize how the model assigns different importance weights to words when predicting answer groups.

## Lab Objectives
- Understand how attention weights are calculated and used in RNNs.
- Preprocess text data using tokenization, encoding, and padding.
- Build and train an RNN model with an attention mechanism.
- Visualize attention weights using bar charts.
- Analyze how attention changes across questions with similar meanings.

## Tasks Completed
- **Task 1 – Understanding Attention Weights:** Visualized attention weights for three different questions and identified the words receiving the highest attention.
- **Task 2 – Comparing Attention for Similar Questions:** Compared attention distributions for two semantically similar questions with different wording.

## Tools and Libraries
- Python
- PyTorch
- Pandas
- Matplotlib
- Google Colab

## Key Learning Outcome
Attention mechanisms allow an RNN model to assign different weights to words based on their relevance to the prediction. The experiments demonstrated that similar questions can produce different attention distributions depending on their wording.
