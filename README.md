<div align="center">
  <img src="logo.png" alt="sandbox-vertex-ai" width="512"/>

  [![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
  [![Python](https://img.shields.io/badge/Python-3.10-3776AB.svg)](https://www.python.org/)
  [![Gemini](https://img.shields.io/badge/Gemini-2.0-4285F4.svg)](https://ai.google.dev/)

  **A sandbox for experimenting with Google's Gemini API**

  [Google AI Studio](https://aistudio.google.com/) · [Gemini Cookbook](https://github.com/google-gemini/cookbook)
</div>

## Overview

This project provides a minimal setup for experimenting with Google's Gemini API using the `google-genai` Python SDK. Perfect for prototyping AI features, testing prompts, and exploring Gemini's capabilities.

## Features

- Simple environment setup with conda
- API key authentication via environment variables or `.env` file
- Ready-to-run example using `gemini-2.0-flash-exp` model

## Quick Start

1. Get your API key from [Google AI Studio](https://aistudio.google.com/app/apikey)

2. Set up environment:
```bash
export GOOGLE_API_KEY="your-api-key-here"
```

3. Create and activate conda environment:
```bash
conda env create -f environment.yml
conda activate vertex-ai
```

4. Run the example:
```bash
python main.py
```

## Usage

The main script demonstrates a simple content generation call:

```python
from dotenv import load_dotenv
load_dotenv()

from google import genai

client = genai.Client()
response = client.models.generate_content(
    model='gemini-2.0-flash-exp',
    contents='How does AI work?'
)
print(response.text)
```

## Configuration

### Environment Variables

| Variable | Required | Description |
|----------|----------|-------------|
| `GOOGLE_API_KEY` | Yes | API key from Google AI Studio |

You can set the API key via:
- Environment variable: `export GOOGLE_API_KEY="your-key"`
- `.env` file in the project root (loaded via python-dotenv)

### Dependencies

| Package | Purpose |
|---------|---------|
| `python-dotenv` | Environment variable management |
| `google-genai` | Google's Gemini API SDK |

## References

- [Gemini Cookbook Examples](https://github.com/google-gemini/cookbook/tree/main/gemini-2)
- [Get API Key](https://aistudio.google.com/app/apikey)
- [Gemini API Documentation](https://ai.google.dev/docs)

## License

[MIT](LICENSE) © 2025 Tiago Silva
