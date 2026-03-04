# Multi-language RAG Chatbot (Strands + AWS Bedrock)

Quick start:

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\\Scripts\\activate
pip install -r requirements.txt

# Put your .txt/.md docs into data/docs
python -m rag.ingest

# run Streamlit UI
streamlit run app.py

# or start backend API (needed for React frontend):
uvicorn api.fastapi_app:app --reload --port 8000
```

Don't forget to install the new dependencies (`fastapi`, `uvicorn`, `python-multipart`) which are already added to `requirements.txt`.

Configure model IDs and region in `config/settings.py` or environment variables.
