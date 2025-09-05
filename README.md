# LLM OpenRouter Client

A lightweight Python client for interacting with OpenRouter-hosted large language models (LLMs) via the `openai` Python SDK.  
This repo provides a simple `llm` class for sending prompts and retrieving responses from models such as **LLaMA-3.1-70B-Instruct**.

---

## Features
- Minimal wrapper class for OpenRouter LLMs
- Simple `prompt()` method for sending user queries
- Built on top of the official `openai` Python SDK
- Easy environment variable integration for API keys

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/llm-openrouter-client.git
cd llm-openrouter-client
```
Install dependencies:

```bash
pip install openai
```

## Setup
You’ll need an API key from OpenRouter.
Set it as an environment variable:
```bash
export OPENROUTER_API_KEY="your_api_key_here"
```

## Usage
```python
import os
from openai import OpenAI
from llm_client import llm  # adjust import as needed

# Initialize client
chatbot = llm()

# Send a prompt
response = chatbot.prompt("Explain quantum computing in simple terms")
print(response)
```
