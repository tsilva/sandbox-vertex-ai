# sandbox-vertex-ai

A sandbox for playing around with the vertex AI api

## References
- [Gemini Cookbook Examples](https://github.com/google-gemini/cookbook/tree/main/gemini-2)
- [Get API Key](https://aistudio.google.com/app/apikey)

## Setup

1. Get your API key from Google AI Studio
2. Set up environment variable:
```bash
export GOOGLE_API_KEY="your-api-key-here"
```

3. Create and activate conda environment:
```bash
conda env create -f environment.yml
conda activate vertex-ai
```

4. Optional: For persistence, add to your ~/.bashrc or ~/.zshrc:
```bash
export GOOGLE_API_KEY="your-api-key-here"
```