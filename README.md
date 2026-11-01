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
| [02-rag-api](02-rag-api/) | RAG API over my profile with Chroma + FastAPI, multi-user `POST /documents` |

Run everything locally: no cloud APIs or keys needed.
