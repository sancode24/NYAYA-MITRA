# NYAYA-MITRA
# Indian Legal Intelligence Agent (RAG-Based)

A high-grounding precision retrieval-augmented generation assistant designed to query the *Bharatiya Nyaya Sanhita (2023)* legal dataset with minimized hallucinations.

## 🧠 Architecture Implementation
- **Two-Stage Retrieval:** Leverages a baseline Bi-Encoder for vector search across semantic embeddings, paired with a Cross-Encoder reranker to optimize retrieval precision.
- **Vector Storage:** Utilizing ChromaDB to house local document embeddings chunked sequentially.
- **Pipeline Resilience:** Built with robust API integration layers utilizing exponential backoff algorithms to safely mitigate endpoint rate limits.

## 🛠️ Tech Stack
- **Language:** Python
- **Orchestration & LLM:** LangChain, Gemini 1.5 Flash
- **Embeddings & Vector Database:** Hugging Face (`MiniLM`), ChromaDB
