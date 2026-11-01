# Part 2: RAG API with FastAPI

Run these from inside `02-rag-api/`.

```bash
python -m venv venv
venv\Scripts\activate                # Windows  (source venv/bin/activate on Linux/macOS)
pip install -r requirements.txt
ollama pull nomic-embed-text
python build_knowledge_base.py
uvicorn main:app --reload
```
Open http://127.0.0.1:8000/docs.

| Endpoint | What it does |
|---|---|
| `GET /ask?question=...` | Retrieves the 2 closest chunks and answers with `qwen2.5:0.5b` |

Response shape: `{"question", "answer", "context_used"}`.

