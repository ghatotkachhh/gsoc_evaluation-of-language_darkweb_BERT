# GSoC Project: Evaluation of Language Models on Dark Web Text using BERT

This repository contains the code and resources for evaluating language models, particularly BERT, on text data extracted from the dark web. The project is part of Google Summer of Code (GSoC).

## Introduction
The dark web presents unique challenges for natural language processing (NLP) tasks due to its unconventional language, structure, and content. This project aims to evaluate the performance of BERT-based language models on such text data. By understanding how well these models perform on dark web text, we can improve their applicability to various security and surveillance tasks.

## Model Weights
The weights of the best-performing models trained as part of this project can be found [here](https://drive.google.com/drive/folders/1etOZP4j-aWjxs_zUOiQiTYyDZkNuPuHm?usp=sharing). 

To load the weights into the model, follow these steps:
```python
import torch

# Replace "directory to the weights" with the actual directory where you've downloaded the weights
weights = torch.load("directory to the weights")
model.load_state_dict(weights["model"])
