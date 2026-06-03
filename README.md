# AI-llm-integration-starter (Gemini & Ollama)

This project is a practical, step-by-step guide inside a Jupyter Notebook that demonstrates how to connect and interact with Large Language Models (LLMs). The core focus is utilizing the standard OpenAI API structure to seamlessly switch between cloud-based providers (like Google Gemini) and local/open-source models (via Ollama).

## Key Features
- Secure Environment Management: Utilizing .env files to prevent API key exposure.
- Unified Client Architecture: Demonstrating how a single client interface (OpenAI Client) can communicate with different AI backends.
- Local LLM Support: Running and testing prompts completely offline on your own machine using Ollama.

## Prerequisites
To run this notebook, you will need:
- Python 3.8 or higher
- Ollama installed and running (for the local model section)

## Getting Started
- Clone the repository.
- Create a .env file in the root directory of the project and configure the following environment variables:

```bash
GEMINI_API_KEY=your_actual_gemini_api_key
GEMINI_BASE_URL=[https://generativelanguage.googleapis.com/v1beta/openai/](https://generativelanguage.googleapis.com/v1beta/openai/)
GEMINI_MODEL=gemini-1.5-flash
OLLAMA_BASE_URL=http://localhost:11434/v1
OLLAMA_MODEL=llama3
```
## Setup
- Using Python + venv

bash:
```BASH
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```
Install Dependensies

- Using UV (recommended)

After selecting the Python version, create a virtual environment with uv:

````
uv venv
````
Then install the dependencies:

````
uv pip install -r requirements.txt --refresh
````