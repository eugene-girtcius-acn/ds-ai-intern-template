## Week 7: Retrieval-Augmented Generation (RAG)

### Retrieval-Augmented Generation
- Vector databases and embeddings (Chroma, Pinecone, FAISS)
- Building RAG systems with public knowledge bases
- Chunking strategies for effective retrieval
- Retrieval strategies (query transformation, reranking, HyDE)
- Hybrid search approaches
- Advanced RAG architectures
- Production considerations for RAG systems

### RAG Evaluation
- Evaluation dimensions (retrieval, generation, end-to-end)
- Evaluation frameworks (RAGAS, DeepEval, Promptfoo, Arize Phoenix)
- Key metrics (Context precision/recall, context relevance, faithfulness, answer relevance)

### Datasets
- [Simple English Wikipedia](https://huggingface.co/datasets/wikipedia)

### Theory, Courses & Additional Reading
- [paper: Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/pdf/2005.11401)
- [paper: Dense Passage Retrieval for Open-Domain Question Answering](https://arxiv.org/pdf/2004.04906)
- [paper: Corrective Retrieval Augmented Generation](https://arxiv.org/abs/2401.15884)
- [paper: From Local to Global: A Graph RAG Approach to Query-Focused Summarization](https://arxiv.org/abs/2404.16130)
- [DeepEval](https://deepeval.com/docs/getting-started)
- [RAGAS](https://docs.ragas.io/en/latest/)
- [course: Embedding Models: From Architecture to Implementation](https://www.deeplearning.ai/short-courses/embedding-models-from-architecture-to-implementation/)
- [course: Retrieval Optimization: From Tokenization to Vector Quantization](https://www.deeplearning.ai/short-courses/retrieval-optimization-from-tokenization-to-vector-quantization/)
- [course: Vector Databases: from Embeddings to Applications](https://www.deeplearning.ai/short-courses/vector-databases-embeddings-applications/)
- [course: Building Applications with Vector Databases](https://www.deeplearning.ai/short-courses/building-applications-vector-databases/)
- [course: Building and Evaluating Advanced RAG Applications](https://www.deeplearning.ai/short-courses/building-evaluating-advanced-rag/)
- [course: Knowledge Graphs for RAG](https://www.deeplearning.ai/short-courses/knowledge-graphs-rag/)

### Assignments
**Assignment 1: Comprehensive RAG System**

Specific Task: Build a small-scale RAG system for answering factual questions

Deliverables:

- Vector database setup with a small subset of Wikipedia articles (e.g., 1000 articles on a specific topic)
- Basic chunking and embedding strategy
- Basic retrieval and generation pipeline
- Simple web interface for questions

Success Criteria: System successfully retrieves relevant context and generates reasonable answers

**Assignment 2: RAG Evaluation Pipeline**

Specific Task: Build an evaluation framework for your RAG system

Deliverables:

- Evaluation dataset: 10+ question-answer pairs for your corpus
- Implement evaluation metrics: RAG Triad, Recall@k, NDCG
- Compare different RAG configurations (embeddings / chunk size, etc.)
- Evaluation report: recommendations for optimal configuration

Success Criteria: Comprehensive evaluation across multiple dimensions