# Week 1 exercise — technical question explainer

Completed end-of-week-1 exercise from Ed Donner's LLM Engineering course.

The notebook takes a technical question (here: a short Python snippet) and returns an explanation from:

1. **GPT-4o-mini** via the OpenAI API, with streaming
2. **Llama 3.2** via a local Ollama server (OpenAI-compatible endpoint)

## Setup

1. Copy the repo-root `.env.example` to `.env` and add your OpenAI API key.
2. Install dependencies (from this folder or the repo root):

   ```bash
   pip install -r requirements.txt
   ```

3. Start Ollama and pull the model used in the notebook:

   ```bash
   ollama serve
   ollama pull llama3.2
   ```

   On a smaller machine, use `llama3.2:1b` instead and change `MODEL_LLAMA` in the notebook.

4. Open `week1 EXERCISE.ipynb` and run all cells.

The notebook looks for `.env` in the current working directory and parent folders, so it works if you launch Jupyter from this `week1` folder or from the repo root.
