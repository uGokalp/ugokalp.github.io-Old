---
layout: archive
title: "Happy Transformer"
permalink: /nlp/

author_profile: true

---

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Downloads](https://pepy.tech/badge/happytransformer)](https://pepy.tech/project/happytransformer)

Happy Transformer is an API built on top of [PyTorch's transformer library](https://pytorch.org/hub/huggingface_pytorch-transformers/) that makes it easy to utilize state-of-the-art NLP models. 

## Key Features
  - **New: Finetuning Masked Language Models**
  - Available language models: XLNET, BERT and ROBERTA.
  - Predict a masked word within a sentence.
  - Fine tune binary sequence classification models to solve problems like sentiment analysis.
  - Predict the likelihood that sentence B follows sentence A within a paragraph. 
  
  
| Public Methods                     | HappyROBERTA | HappyXLNET | HappyBERT |
|------------------------------------|--------------|------------|-----------|
| Masked Word Prediction             | ✔            | ✔          | ✔         |
| Sequence Classification            | ✔            | ✔          | ✔         |
| Next Sentence Prediction           |              |            | ✔         |
| Question Answering                 |              |            | ✔         |
| Masked Word Prediction Finetuning  | ✔            |            | ✔         |


*I have contributed directly to Masked Word Prediction and Masked Word Prediction Finetuning.*