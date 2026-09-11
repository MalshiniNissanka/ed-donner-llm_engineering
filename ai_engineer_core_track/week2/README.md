# Week 2

One notebook: `week2.ipynb`

1. Prompt caching — long static prefix first, variable content last
2. Multi-turn conversation between two models — Gemini and local Ollama
3. Chat history and the system prompt — the `system + history + message` callback
4. Multimodal — image sent to Gemini as a base64 data URL
5. Tools — function calling with a Python docs lookup
6. Prototype — the Week 1 explainer as a Gradio app: streaming, expert system prompt, model switch, tool calling

```bash
pip install -r ../week1/requirements.txt
pip install gradio pillow
ollama serve
ollama pull qwen2.5:0.5b
```

`.env` in the repo root needs `OPENAI_API_KEY` and `GOOGLE_API_KEY`. Run all cells; the last one opens the Gradio UI.
