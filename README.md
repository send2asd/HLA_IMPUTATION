# Ajay Singh
## Master of Science in Computer Science
### HLA IMPUTATION USING MACHINE LEARNING
### Overview
- This project focuses on implementing a sequence-to-sequence model with attention mechanism using PyTorch. The model is designed to translate sentences from a source language to a target language. The dataset used for this task contains pairs of sentences in a low-resource language (source) and its corresponding English translation (target).

### Project Structure
#### Data Preprocessing
- The initial step involves cleaning and preprocessing the dataset. The data is loaded from a text file ('data/low-high.txt'), and sentences are formatted to be tokenized and converted into numerical indices. The dataset is split into training and testing sets.

#### Model Architecture
- The implemented model consists of an encoder and a decoder. The encoder processes the input sequence and produces context vectors, while the decoder generates the output sequence using these context vectors. The attention mechanism allows the model to focus on different parts of the input sequence during the decoding process.

#### Training
- The training process involves optimizing the model's parameters using the Adam optimizer and minimizing the negative log likelihood loss. The model is trained for a specified number of epochs, with periodic printing of loss values for monitoring.

#### Code Organization
preprocess.py: Contains functions for data loading, preprocessing, and creating PyTorch dataloaders.
models.py: Defines the architecture for the encoder, decoder, and attention mechanism.
train.py: Implements the training loop for the sequence-to-sequence model.
evaluate.py: Includes functions for evaluating the model on random examples.

#### Usage
#### Data Preprocessing:
```python preprocess.py```

#### Training:
```python train.py```


#### Evaluation:
```python evaluate.py```

#### Results
- The trained model is evaluated on random examples to observe its translation performance. Adjustments to hyperparameters and model architecture can be made for further improvements.

#### Dependencies
- Python 3.x
PyTorch
NumPy
Notes
Ensure that the necessary data files are available in the specified directories.
Training and evaluation parameters can be adjusted in the respective scripts.
