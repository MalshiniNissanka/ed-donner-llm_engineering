# Week 1 exercise — technical question explainer

Takes a technical question and streams an explanation from each model:

| Model | Provider |
|---|---|
| `gpt-4o-mini` | OpenAI |
| `gemini-3.1-flash-lite` | Google |
| `claude-haiku-4-5` | Anthropic |
| `qwen2.5:0.5b` | Ollama, local |

Every provider is called through the OpenAI client, since Google, Anthropic and Ollama all expose OpenAI-compatible endpoints. Only the `base_url` changes.

## Setup

Add your keys to `.env` in the repo root:

```
OPENAI_API_KEY=...
GOOGLE_API_KEY=...
ANTHROPIC_API_KEY=...
```

Install dependencies and start the local model:

```bash
pip install -r requirements.txt
ollama serve
ollama pull qwen2.5:0.5b
```

Then open `week1 EXERCISE.ipynb`, select the Python kernel, and Run All.
