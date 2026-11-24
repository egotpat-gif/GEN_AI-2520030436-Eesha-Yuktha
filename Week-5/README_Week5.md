# Week 5 - Token Economics and Budget Planning

## About
In this week, I created a simple Python tool to estimate the token usage and cost of an LLM feature before building it.

The tool also checks whether the expected requests and token usage fit within the given rate limits and budget.

## What I Used
- Python
- VS Code
- python-dotenv
- unittest

## Main Files
- `budget.py` - Calculates token usage, estimated cost, and limit checks.
- `test_budget.py` - Tests the calculations and checks.
- `.env` - Stores the sample usage, price, budget, and rate-limit values.
- `requirements.txt` - Lists the required Python package.

## What the Tool Calculates
- Input tokens per day
- Output tokens per day
- Total tokens per day
- Estimated daily cost
- Estimated monthly cost
- Requests per minute (RPM)
- Tokens per minute (TPM)
- Daily and monthly budget checks

## How It Works
1. The program reads the planning values from `.env`.
2. It calculates the expected daily and monthly token usage.
3. It estimates the API cost using the input and output token prices.
4. It applies a safety margin.
5. It checks the RPM, TPM, daily budget, and monthly budget.
6. It prints a report with PASS or REVIEW results and a recommendation.

## How to Run
Install the required package:

```bash
pip install -r requirements.txt
```

Run the budget planner:

```bash
python budget.py
```

Run the tests:

```bash
python -m unittest test_budget.py
```

## Note
The prices and limits in `.env` are sample planning values. Update them using the correct prices and limits for the model and account being used. The estimate is not a final bill.
