# Personal RAG API

A small Retrieval-Augmented Generation API that answers questions about my profile. It runs fully locally: **Ollama** serves the models, **Chroma** stores the embeddings and **FastAPI** exposes the endpoints.

## Stack
- Ollama: `qwen2.5:0.5b` (chat), `nomic-embed-text` (embeddings), `gemma3:1b` (custom `coding-tutor` model)
- ChromaDB (persistent, `./chroma_db`)
- FastAPI + Uvicorn

## Projects
| Folder | Project |
|---|---|
| [01-ollama-local](01-ollama-local/) | Run an LLM locally with Ollama, plus a custom `coding-tutor` model |
| [Rag-Api-with-FAST-API](https://github.com/Harjeet2411/Rag-Api-with-FAST-API) (own repo) | RAG API over my profile with Chroma + FastAPI, multi-user `POST /documents` |

Run everything locally: no cloud APIs or keys needed.
