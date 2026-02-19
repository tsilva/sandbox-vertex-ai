# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a sandbox project for experimenting with Google's Gemini API (formerly Vertex AI). The project uses the `google-genai` Python SDK to interact with Gemini models.

## Environment Setup

The project uses conda for environment management:

```bash
# Create and activate the environment
conda env create -f environment.yml
conda activate vertex-ai
```

## Authentication

The project requires a Google API key from [Google AI Studio](https://aistudio.google.com/app/apikey):

```bash
export GOOGLE_API_KEY="your-api-key-here"
```

The API key can be loaded via environment variable or `.env` file (using python-dotenv).

## Running Code

Execute the main example:

```bash
python main.py
```

## Key Dependencies

- `python-dotenv`: Environment variable management
- `google-genai`: Google's Gemini API SDK (Python 3.10)

## Architecture Notes

- The project uses the `google.genai.Client()` interface to interact with Gemini models
- Current example uses `gemini-2.0-flash-exp` model
- API key authentication is handled via environment variables loaded through dotenv

## Important Instructions

- README.md must be kept up to date with any significant project changes
