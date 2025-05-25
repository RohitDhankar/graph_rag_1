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


------------------------------------

* **GitHub Repository**: [neo4j/neo4j-graphrag-python](https://github.com/neo4j/neo4j-graphrag-python)
* **Official Documentation**: [Neo4j GraphRAG Python Docs](https://neo4j.com/docs/neo4j-graphrag-python/current/)
* **Installation**:

```bash
  pip install neo4j-graphrag
```

------------------------------------

###### Additional Refrences 

[1]: https://neo4j.com/blog/developer/get-started-graphrag-python-package/?_"Getting Started with Neo4j GraphRAG Python Package"
[2]: https://neo4j.com/docs/neo4j-graphrag-python/current/?_"neo4j-graphrag-python documentation"
[3]: https://github.com/neo4j/neo4j-genai-python/blob/main/.editorconfig?_"neo4j-graphrag-python/.editorconfig at main - GitHub"
[4]: https://neo4j.com/labs/genai-ecosystem/graphrag-python/?_"Neo4j GraphRAG Python Package - Neo4j Labs"
[5]: https://neo4j.com/blog/developer/enhancing-hybrid-retrieval-graphrag-python-package/?_"Enhancing Hybrid Retrieval With Graph Traversal: Neo4j GraphRAG ..."


------------------------------------
