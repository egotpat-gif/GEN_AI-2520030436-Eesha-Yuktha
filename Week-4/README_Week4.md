# Week 4 - Tokenizer Comparison

## About
In this week, I compared three tokenizers: BPE, WordPiece, and SentencePiece.

I used the same English, Telugu, and Hindi sentences with all three tokenizers. The program displays the tokens, token IDs, and total token count for each sentence.

## What I Used
- Python
- Hugging Face Transformers
- SentencePiece
- VS Code

## Main Files
- `tokenizer_comparison.py` - Loads the tokenizers and compares their results.
- `requirements.txt` - Contains the required Python packages.

## Tokenizers Used
- BPE - GPT-2
- WordPiece - Multilingual BERT
- SentencePiece - XLM-R

## How It Works
1. The program loads the three pretrained tokenizers.
2. It takes English, Telugu, and Hindi sentences as input.
3. Each tokenizer splits the same sentence into smaller tokens.
4. The program displays the token pieces, token IDs, and token count.
5. The results can be compared to see how each tokenizer handles different languages.

## How to Run
Install the required packages:

```bash
pip install -r requirements.txt
```

Run the program:

```bash
python tokenizer_comparison.py
```

The first run may need an internet connection to download the pretrained tokenizer files.

## Result
This practical shows that different tokenizers can split the same sentence in different ways. Token counts depend on the tokenizer and the vocabulary used by its model.
