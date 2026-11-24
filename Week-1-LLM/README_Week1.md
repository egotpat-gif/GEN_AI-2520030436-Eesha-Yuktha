# Week 1 - First LLM API Call

## About
In this week, I created a simple Python program that connects to Google's Gemini AI using the Gemini API.

The program sends a question to Gemini and displays the answer in the VS Code terminal.

## What I Used
- Python
- Gemini API
- VS Code
- python-dotenv
- google-genai

## Files
- `main.py` - Connects to Gemini, sends a prompt, and prints the response.
- `.env` - Stores the Gemini API key.
- `.gitignore` - Prevents private and unnecessary files from being uploaded.
- `requirements.txt` - Contains the Python packages needed for the project.

## How It Works
1. The program reads the Gemini API key from the `.env` file.
2. It connects to the Gemini model.
3. It sends a prompt to the model.
4. Gemini generates an answer.
5. The answer is displayed in the terminal.

## How to Run
Install the required packages:

```bash
pip install -r requirements.txt
```

Run the program:

```bash
python main.py
```

## Note
Keep your Gemini API key private. Do not upload the `.env` file to GitHub.
