# graph_rag_1

Target is to build a open-source solution for building a Graph RAG 
(Retrieval-Augmented Generation) system using fully open-source tools and libraries

Initial Options being considered and experimentes with are - 

**1. Knowledge Graph Backend**:
- **Neo4j** (graph database) + **APOC** (plugin)
- **Alternative**: ArangoDB (multi-model graph database)

**2. NLP/LLM Components**:
- **LangChain** (orchestration)
- **LlamaIndex** (retrieval)
- **HuggingFace Transformers** (local LLMs)
- **Sentence Transformers** (embeddings)

**3. Vector Search**:
- **FAISS** (Facebook AI Similarity Search)
- **Weaviate** (open-source vector search)

**4. Deployment**:
- **FastAPI** (backend)
- **Streamlit** (frontend)
- **Docker** (containerization)