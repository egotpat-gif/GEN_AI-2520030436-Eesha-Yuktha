# Week 3 - LLM Monitoring with MongoDB

## About
In this week, I improved the LLM application by adding monitoring with MongoDB.

The program records information about LLM requests, such as token usage, response time, estimated cost, and whether the request was successful or failed.

## What I Used
- Python
- Gemini API
- Ollama
- MongoDB Atlas
- VS Code
- python-dotenv
- PyMongo
- requests

## Main Files
- `main.py` - Lets the user choose Gemini or Ollama and enter a prompt.
- `llm_client.py` - Sends prompts to the selected model and handles requests.
- `usage_logger.py` - Saves usage details in MongoDB.
- `test_client.py` - Tests the client using a fake provider and logger.
- `.env` - Stores the Gemini API key and MongoDB connection string.
- `requirements.txt` - Lists the required Python packages.

## How It Works
1. The user selects Gemini or Ollama.
2. The program sends the prompt to the selected model.
3. It records the token usage and time taken for the response.
4. It estimates the Gemini API cost using the configured token prices.
5. It saves request details in MongoDB.
6. It uses timeouts and limited retries to handle temporary errors.

## How to Run
Install the required packages:

```bash
pip install -r requirements.txt
```

Run the program:

```bash
python main.py
```

For Ollama, make sure Ollama is running and the required model is downloaded.

## Note
Add your own Gemini API key and MongoDB connection string to `.env`. Never upload `.env` or share your passwords and API keys on GitHub.
