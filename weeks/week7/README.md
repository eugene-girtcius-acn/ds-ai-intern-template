## Week 7: RAG & AI Agents

### Retrieval-Augmented Generation
- Vector databases and embeddings (Chroma, Pinecone, FAISS)
- Building RAG systems with public knowledge bases
- Chunking strategies for effective retrieval
- Hybrid search approaches
- Evaluating RAG system performance
- Advanced RAG architectures
- Production considerations for RAG systems

### AI Agents Fundamentals
- Introduction to the agent paradigm
- ReAct (Reasoning + Acting) pattern
- Tool use and function calling with LLMs
- Planning and decomposition strategies
- Implementing memory for agents
- Multi-agent systems
- Agent frameworks overview (LangGraph, CrewAI)
- Integrating RAG with agents

### Datasets
- [Simple English Wikipedia](https://huggingface.co/datasets/wikipedia)
- [HotpotQA](https://huggingface.co/datasets/hotpot_qa)

### Theory, Courses & Additional Reading
- [paper: Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/pdf/2005.11401)
- [paper: Dense Passage Retrieval for Open-Domain Question Answering](https://arxiv.org/pdf/2004.04906)
- [paper: ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/pdf/2210.03629)
- [paper: Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/pdf/2304.03442)
- [course: Embedding Models: From Architecture to Implementation](https://www.deeplearning.ai/short-courses/embedding-models-from-architecture-to-implementation/)
- [course: Retrieval Optimization: From Tokenization to Vector Quantization](https://www.deeplearning.ai/short-courses/retrieval-optimization-from-tokenization-to-vector-quantization/)
- [course: Vector Databases: from Embeddings to Applications](https://www.deeplearning.ai/short-courses/vector-databases-embeddings-applications/)
- [course: Building Applications with Vector Databases](https://www.deeplearning.ai/short-courses/building-applications-vector-databases/)
- [course: Building and Evaluating Advanced RAG Applications](https://www.deeplearning.ai/short-courses/building-evaluating-advanced-rag/)
- [course: Welcome to the 🤗 AI Agents Course - Hugging Face Agents Course](https://huggingface.co/learn/agents-course/unit0/introduction)
- [course: AI Agents in LangGraph](https://www.deeplearning.ai/short-courses/ai-agents-in-langgraph/)
- [course: Building Agentic RAG with LlamaIndex](https://www.deeplearning.ai/short-courses/building-agentic-rag-with-llamaindex/)
- [course: Multi AI Agent Systems with crewAI](https://www.deeplearning.ai/short-courses/multi-ai-agent-systems-with-crewai/)
- [course: AI Agentic Design Patterns with AutoGen](https://www.deeplearning.ai/short-courses/ai-agentic-design-patterns-with-autogen/)

### Assignments
**Assignment 1: Comprehensive RAG System**

Specific Task: Build a small-scale RAG system for answering factual questions

Deliverables:

- Vector database setup with a small subset of Wikipedia articles (e.g., 1000 articles on a specific topic)
- Basic chunking and embedding strategy
- Basic retrieval and generation pipeline
- Simple web interface for questions

Success Criteria: System successfully retrieves relevant context and generates reasonable answers

**Assignment 2: Task Completion Agent**

Specific Task: Enhance the RAG system with agent capabilities

Deliverables:

- Build upon the previous RAG implementation
- Add 2-3 basic tools (e.g., router, search query refinement, calculator)
- Implement a basic reasoning step before generating answers
- Create a simple way to log the agent's steps

Success Criteria: Successfully use tools to enhance answers when appropriate
