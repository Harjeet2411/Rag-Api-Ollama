# Part 1 screenshots: run a model locally with Ollama

## 1. Check the Ollama version
`ollama --version` shows Ollama is installed.

![ollama --version](01-ollama-version.png)

## 2. Check the Ollama server
`curl http://localhost:11434` returns "Ollama is running".

![Ollama is running](02-ollama-running.png)

## 3. Pull qwen2.5:0.5b
Download the small Qwen 2.5 chat model.

![ollama pull qwen2.5:0.5b](03-pull-qwen.png)

## 4. Ask a general question
The model answers "What is the capital of France?" correctly.

![Capital of France](04-run-capital-of-france.png)

## 5. Ask a personal question
The model has no context about me, so it cannot know my name.

![What's my name](05-run-whats-my-name.png)

## 6. Pull gemma3:1b
Download the base model for the custom tutor.

![ollama pull gemma3:1b](06-pull-gemma3.png)

## 7. Create the coding-tutor model
Build a custom model from `modelfiles/coding-tutor` (system prompt + temperature).

![ollama create coding-tutor](07-create-coding-tutor.png)

## 8. Run the coding-tutor model
The tutor explains list comprehensions step by step and ends with a follow-up question.

![ollama run coding-tutor](08-run-coding-tutor.png)

## 9. List local models
`ollama list` shows qwen2.5:0.5b, gemma3:1b and coding-tutor.

![ollama list](09-ollama-list.png)
