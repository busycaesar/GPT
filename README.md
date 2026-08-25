# GPT

> 🚧 Work in Progress — this project is under active development.

## Description

A character-level GPT (Generatively Pretrained Transformer) built from scratch, trained on the [tiny-shakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt) dataset.

This project is inspired by Andrej Karpathy's video [Let's build GPT: from scratch, in code, spelled out.](https://www.youtube.com/watch?v=kCc8FmEb1nY)

## Tech Stack

![Image Alt](https://skillicons.dev/icons?i=py,pytorch,jupyter)

## Workflow

This project walks through the full pipeline of building a character-level GPT from scratch:

1. Downloads and loads the tiny-shakespeare dataset for training
2. Tokenizes text at the character level, converting between raw text and numeric token sequences
3. Splits the dataset into training and validation sets
4. Samples random batches of context and target sequences for training
5. Trains a bigram language model, where each token directly predicts the next token's probabilities, using an AdamW optimizer running on a GPU when one is available
6. Periodically evaluates and reports the model's averaged training and validation loss during training
7. Generates new text by repeatedly sampling one token at a time from the trained model

All training hyperparameters, such as batch size, context length, iteration count, and learning rate, are centralized in one place.

## How to run the project?

1. Clone the repository
2. Install dependencies: `pip install torch`
3. Open `main.ipynb` in Jupyter and run the cells, or run the plain script version with `python main.py`

## Author

[Dev J. Shah](https://github.com/busycaesar)
