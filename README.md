This project involves building and training recurrent neural networks (RNNs) for various text sequence generation tasks. It was completed as part of the **INF265** course and focuses on exploring sequence data, RNNs, attention mechanisms, word embeddings, and text generation.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Tasks Breakdown](#tasks-breakdown)
    - [Word Embedding](#word-embedding)
    - [Conjugating Be and Have](#conjugating-be-and-have)
    - [Text Generation](#text-generation)
3. [Models and Architectures](#models-and-architectures)
    - [RNN](#rnn)
    - [Attention Layer](#attention-layer)
4. [Installation and Setup](#installation-and-setup)
5. [Results and Evaluation](#results-and-evaluation)
6. [Usage](#usage)
7. [Acknowledgements](#acknowledgements)

## Project Overview

The project is centered on text sequence generation using RNN-based models. The primary objectives are:
- Understanding and working with sequence data.
- Training models to predict text sequences.
- Implementing attention mechanisms to enhance model performance.
- Utilizing word embeddings to improve textual representations.

The project is divided into three main sections, each targeting different aspects of sequence modeling.

## Tasks Breakdown

### Word Embedding
1. **Tokenization**: Read and tokenize text data to prepare for embedding generation.
2. **Vocabulary Creation**: A vocabulary was created from the training dataset, where only words that appear at least 100 times are included.
3. **Embedding Model**: A continuous bag of words (CBOW) model was used to create word embeddings with a small dimension size (e.g., 16, 12).
4. **Evaluation**: Cosine similarity was computed to find the most similar words in the vocabulary, and the embedding space was visualized using TensorFlow's projector tool.

### Conjugating Be and Have
1. **Task**: Predicting the correct conjugation of "be" and "have" given the surrounding context.
2. **Models**: An MLP, an attention-based MLP, and an RNN were trained and compared for performance.
3. **Evaluation**: The models were evaluated based on their ability to correctly conjugate the verbs and the differences in training times and performance.

### Text Generation
1. **Task**: Generating text sequences based on the preceding context.
2. **Models**: RNNs were used to predict the next word in a sequence, and a beam search algorithm was implemented for improved sentence completion.
3. **Results**: The model was tested with various starting sequences, and its output was evaluated for coherence and relevance.

## Models and Architectures

### RNN
Recurrent neural networks were used to model sequences where the length of the input and output sequences may vary. The RNN shares weights across different positions in the sequence.

### Attention Layer
A simple attention mechanism was implemented to focus on the most relevant parts of the input sequence. Multi-head attention was also explored, which allows the model to consider multiple parts of the input simultaneously.

## Installation and Setup

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Required Python Libraries: 
  - `pandas`
  - `numpy`
  - `torch`
  - `matplotlib` (for visualization)
  - Other dependencies listed in `requirements.txt`

### Setup

1. Clone the repository:
```bash
git clone https://github.com/username/repo-name.git
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Run the Jupyter notebook:
```bash
jupyter notebook
```

## Results and Evaluation

The project yielded various insights into the performance of different models:

Word Embedding: Visualized clusters of similar words.
Conjugation Task: Noted performance differences between MLPs and RNNs, with attention-based models performing slightly better.
Text Generation: The generated text was syntactically correct, though semantic coherence was limited due to the scope of the task.

## Acknowledgements

This project was developed as part of the INF265 course at the University of Bergen.


## Contact

Khalil Ibrahim - [GitHub](https://github.com/KhalilIbrahimm)
