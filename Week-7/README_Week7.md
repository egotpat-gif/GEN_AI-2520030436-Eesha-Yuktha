# Week 7 - Next-Token Probability Analysis

## About
In this week, I created a Python program to understand how a language model predicts the next word or token.

The program uses the GPT-2 model. It takes a few sample prompts, checks the possible next tokens, and displays the top 5 predictions with their probabilities.

## What I Used
- Python
- GPT-2
- PyTorch
- Hugging Face Transformers
- VS Code
- CSV

## Main Files
- `main.py` - Loads GPT-2, checks the next-token predictions for each prompt, and saves the results.
- `requirements.txt` - Lists the Python packages needed for the project.
- `week7_probability_results.csv` - Stores the prompts, predicted tokens, token IDs, and probabilities created by the program.

## How It Works
1. The program loads the GPT-2 model and tokenizer.
2. It uses four sample prompts.
3. The tokenizer converts each prompt into token IDs.
4. GPT-2 predicts possible next tokens.
5. The program converts the model's logits into probabilities.
6. It displays the top 5 next-token candidates and their probabilities.
7. It saves the results in a CSV file.

## How to Run
Install the required packages:

```bash
pip install -r requirements.txt
```

Run the program:

```bash
python main.py
```

The first run may need an internet connection to download the GPT-2 model and tokenizer.

## Result
The program displays the top 5 possible next tokens for each prompt, along with their token IDs and probabilities.

It also creates a file named `week7_probability_results.csv` containing all the results.

## Note
The probabilities show how likely the model considers each next token for the given prompt. They are model predictions and do not guarantee that the generated text will be correct or meaningful.
