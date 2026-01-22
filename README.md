<div align="center">
  <img src="logo.png" alt="sandbox-vertex-ai" width="512"/>

  **💎 Sandbox for experimenting with Google's Gemini API**

</div>

## Overview

A sandbox project for experimenting with Google's Gemini API (formerly Vertex AI). Uses the `google-genai` Python SDK to interact with Gemini models.

## Features

- **Gemini integration** - Direct access to Gemini models
- **Simple API** - Uses `google.genai.Client()` interface
- **Environment config** - API key via `.env` file

## Quick Start

```bash
# Clone and setup
git clone https://github.com/tsilva/sandbox-vertex-ai.git
cd sandbox-vertex-ai

# Create environment
conda env create -f environment.yml
conda activate vertex-ai

# Configure API key
cp .env.example .env
# Edit .env with your GOOGLE_API_KEY from AI Studio

# Run the example
python main.py
```

## Get API Key

1. Visit [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Create an API key
3. Add to `.env` file

## Requirements

- Python 3.10
- Conda
- Google API key

## License

MIT
