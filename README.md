# rag-arxiv-rag
A Retrieval-Augmented Generation (RAG) system that answers questions using real arXiv papers, with grounded responses and citations. First, it ingests the arXiv papers , extracts and clean them using PyMuPDF and chunks the document . I then perform seacrh on Chroma DB using embeddings . Lastly, I used the OpenAI API to create LLM-generated answers grounded in retrived evidence with citations.


Example Query:

What retrieval strategies are commonly used in RAG systems?

Output:
	•	Dense retrieval (e.g., DPR) [1]
	•	Hybrid retrieval (BM25 + dense) [2]
	•	Re-ranking with cross-encoders [3]

## Setup
Run : pip install -r requirements.txt and then the notebook.
