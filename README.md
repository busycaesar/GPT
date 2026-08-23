# GPT

> 🚧 Work in Progress — this project is under active development.

## Description

A character-level GPT (Generatively Pretrained Transformer) built from scratch, trained on the [tiny-shakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt) dataset.

This project is inspired by Andrej Karpathy's video [Let's build GPT: from scratch, in code, spelled out.](https://www.youtube.com/watch?v=kCc8FmEb1nY)

## Tech Stack

![Image Alt](https://skillicons.dev/icons?i=py,pytorch,jupyter)

## Features

- Downloads and loads the tiny-shakespeare dataset
- Builds a character-level tokenizer (`encode`/`decode`)
- Splits the dataset into training and validation sets
- Batches random context/target chunks for training (`get_batch`)
- Implements a `BigramLanguageModel` (an embedding table used directly as next-token logits)
- Generates new text by sampling one token at a time from the model
- Trains the model with an AdamW optimizer and prints the loss

## How to run the project?

1. Clone the repository
2. Install dependencies: `pip install torch`
3. Open `main.ipynb` in Jupyter and run the cells, or run the plain script version with `python main.py`

## Author

[Dev J. Shah](https://github.com/busycaesar)
