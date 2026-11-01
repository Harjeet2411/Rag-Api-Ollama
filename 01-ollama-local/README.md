# Part 1: Run a model locally with Ollama

```bash
curl http://localhost:11434          # "Ollama is running"
ollama pull qwen2.5:0.5b
ollama run qwen2.5:0.5b              # try "What is the capital of France?"
ollama pull gemma3:1b
ollama create coding-tutor -f modelfiles/coding-tutor
ollama run coding-tutor
```


## Screenshots
See [screenshots/README.md](screenshots/README.md).
