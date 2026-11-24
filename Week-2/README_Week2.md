# Week 2 - Provider-Agnostic LLM Client

## About
In this week, I created a Python program that can connect to two different language model providers: Gemini and Ollama.

Gemini is an online AI service, while Ollama runs an AI model locally on the computer. The program allows the user to choose which provider to use and enter a question.

## What I Used
- Python
- Gemini API
- Ollama
- Llama 3.2 model
- VS Code
- python-dotenv
- google-genai
- requests
- pytest

## Main Files
- `main.py` - Asks the user to choose Gemini or Ollama, accepts a question, and displays the answer.
- `llm_client.py` - Contains the common interface and the code for connecting to Gemini and Ollama.
- `test_client.py` - Tests the LLM client using a fake provider.
- `.env` - Stores the Gemini API key.
- `requirements.txt` - Lists the Python packages needed for the project.

## How It Works
1. The program asks the user to choose Gemini or Ollama.
2. If Gemini is selected, the program uses the Gemini API key from the `.env` file.
3. If Ollama is selected, the program uses the locally installed Llama 3.2 model.
4. The user enters a question.
5. The selected model generates an answer.
6. The answer is displayed in the terminal.

## How to Run
Install the required packages:

```bash
pip install -r requirements.txt
```

Make sure Ollama is installed and the Llama 3.2 model is downloaded if you want to use Ollama:

```bash
ollama pull llama3.2
```

Run the program:

```bash
python main.py
```

Run the test:

```bash
python -m unittest test_client.py
```

## Note
Add your Gemini API key to the `.env` file if you want to use Gemini. Keep the API key private and do not upload the `.env` file to GitHub.
