# Week 6 - LLM Golden Question Set Evaluation

## About
In this week, I created a Python program to test how well an AI model answers a set of prepared questions.

The program uses the Llama 3.2 model through Ollama. It checks the model's answers by looking for important keywords and saves the results in a CSV file.

## What I Used
- Python
- Ollama
- Llama 3.2 model
- VS Code
- JSON
- CSV
- requests

## Main Files
- `main.py` - Sends questions to the Llama 3.2 model, checks the answers, calculates scores, and saves the results.
- `golden_set.json` - Contains the questions, expected answers, keywords, and source links.
- `requirements.txt` - Lists the Python package needed for the project.
- `baseline_results.csv` - Stores the evaluation results created by the program.

## How It Works
1. The program loads the questions from `golden_set.json`.
2. It sends each question to the Llama 3.2 model using Ollama.
3. The model generates an answer for each question.
4. The program compares the answer with the expected keywords.
5. It calculates a keyword score for each answer.
6. It marks each result as PASS, REVIEW, or ERROR.
7. It saves the answers and scores in `baseline_results.csv`.
8. It displays a summary of the evaluation in the terminal.

## How to Run
Make sure Ollama is installed and the Llama 3.2 model is downloaded:

```bash
ollama pull llama3.2
```

Install the required package:

```bash
pip install -r requirements.txt
```

Run the program:

```bash
python main.py
```

## Result
The program creates a file named `baseline_results.csv`. It contains the questions, expected answers, model answers, matched and missing keywords, scores, status, source, model name, and release version.

The first evaluation is recorded as Release v0.1.

## Note
Make sure Ollama is running before starting the program. The evaluation uses keyword matching, so the score shows keyword coverage and does not fully measure the meaning or quality of an answer.
