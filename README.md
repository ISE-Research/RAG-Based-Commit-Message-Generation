# Automatic Commit Message Generation using Retrieval-Augmented Generation (RAG)

This repository contains a comprehensive implementation of **Automatic Commit Message Generation** using **Retrieval-Augmented Generation (RAG)** techniques. The project explores different programming languages (`Java`, `JavaScript`, and `Python`) and multiple pre-trained transformer models, including **BART** and **T5**, to enhance version control documentation accuracy and efficiency.

## Overview

The objective of this repository is to automate the process of commit message generation by leveraging RAG to combine powerful language modeling with contextual retrieval. The repository is divided into modules corresponding to each language and framework:

- **Languages**: Java, JavaScript, Python
- **Models**: T5, BART
- **Frameworks**: Hugging Face Transformers, PyTorch, TensorFlow

This project is structured to provide a unified methodology for commit message generation across diverse codebases and workflows.

---

## Key Features

- **Multi-Language Support**: Implements models for generating commit messages for codebases in Java, JavaScript, and Python.
- **RAG Integration**: Combines generative capabilities with contextually retrieved information to improve the quality of generated messages.
- **Pre-trained Transformer Models**: Uses BART and T5 for fine-tuning on commit message datasets.
- **Performance Metrics**: Evaluates results using **BLEU**, **METEOR**, **ROUGE**, **accuracy**, and **readability**.
- **Datasets**: Includes processed datasets (`py.jsonl`, `java.jsonl`, and `js.jsonl`) containing code diffs and corresponding commit messages.

---

## Repository Structure

```plaintext
├── datasets/
│   ├── py.jsonl         # Python dataset with diffs and commit messages
│   ├── java.jsonl       # Java dataset with diffs and commit messages
│   ├── js.jsonl         # JavaScript dataset with diffs and commit messages
├── notebooks/
│   ├── generated_messages_BART_py.ipynb   # BART implementation for Python
│   ├── RAG_BART_Joint_Training_js.ipynb   # BART implementation for JavaScript with RAG
│   ├── RAG_T5_java.ipynb                  # T5 implementation for Java with RAG
│   ├── RAG_T5_js.ipynb                    # T5 implementation for JavaScript with RAG
│   ├── RAG_T5_py.ipynb                    # T5 implementation for Python with RAG
├── models/
│   ├── T5/
│   ├── BART/
└── README.md
