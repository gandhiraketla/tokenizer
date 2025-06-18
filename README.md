# BPE Tokenizer

A simple Byte Pair Encoding (BPE) tokenizer implementation from scratch in Python.

## What it does

- Reads text from PDF files
- Trains a BPE tokenizer by learning frequent character pairs
- Converts words into subword tokens with unique IDs
- Can save/load the trained tokenizer

## Setup

```bash
pip install PyMuPDF
```

## Usage

1. Put your PDF file as `sample_corpus.pdf` in the same directory
2. Run the Jupyter notebook cells in order
3. The tokenizer will train and show examples

## Example

```python
# Training output
Merge 1: ('e', '</w>') (frequency: 1247)
Merge 2: ('t', 'h') (frequency: 891)

# Tokenization
'language' -> ['l', 'a', 'n', 'g', 'u', 'a', 'g', 'e</w>']
Token IDs: [15, 2, 8, 12, 9, 2, 12, 1]
```

## Files

- `bpe_tokenizer.ipynb` - Main implementation
- `sample_corpus.pdf` - Your training data
- `bpe_tokenizer.txt` - Saved tokenizer (auto-generated)
