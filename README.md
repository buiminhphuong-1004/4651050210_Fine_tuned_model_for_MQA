# My Fined-tuned model for Medical question answering problem

## Overview
This project demonstrates training and testing a simple medical QA model that answers questions with **Yes / No / Maybe**.  
All files are stored directly in the `main` branch for simplicity.

## Repository Contents
- `code_train_model.ipynb`: Jupyter notebook for training the model.
- `code_test_model.ipynb`: Jupyter notebook for testing and evaluation.
- `Experimental_Data.json`: Test dataset used for evaluation.
- `config.json`: Model configuration file.
- `generation_config.json`: Generation settings for inference.
- `tokenizer.json`: Tokenizer vocabulary.
- `tokenizer_config.json`: Tokenizer configuration.
- `README.md`: Documentation of the project.

## How to Run
1. Open `code_train_model.ipynb` to train the model.
2. Open `code_test_model.ipynb` to evaluate the model using `Experimental_Data.json` and show the demo interface of the model.
3. Model configuration and tokenizer files are loaded automatically from the repo.

## Experimental Data
The dataset is stored in `Experimental_Data.json`.  
Each entry contains:
- `context`: medical background text
- `question`: related medical question
- `answer`: label (`yes`, `no`, or `maybe`)

### Example
```json
{
  "context": "Aspirin is commonly used as an antipyretic to reduce fever.",
  "question": "Does aspirin reduce fever?",
  "answer": "yes"
}
