# GSoC Project: Evaluation of Language Models on Dark Web Text using BERT

This repository contains the code and the model weights based on the validation loss for the evaluation task for contributing to the project "Evaluation of Language Models on Dark Web Text using BERT". The project is part of Google Summer of Code (GSoC).


## Notebook for the data analysis,preprocessing,training and inference  
The notebook is in the repository named gsoc-eval-test (1).ipynb


## Model Weights
The weights of the best-performing models trained as part of this project can be found [here](https://drive.google.com/drive/folders/1etOZP4j-aWjxs_zUOiQiTYyDZkNuPuHm?usp=sharing). 

To load the weights into the model, follow these steps:
```python
import torch

# Replace "directory to the weights" with the actual directory where you've downloaded the weights
weights = torch.load("directory to the weights")
model.load_state_dict(weights["model"])
