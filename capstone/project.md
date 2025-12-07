# GenAI Mini-Project: Multi-Agent Research System

## Overview

**Duration**: 4 weeks
**Format**: Iterative project with weekly milestones  
**End Goal**: A multi-agent system of your choice that incorporates RAG, intelligent routing, and tool use

This mini-project is an alternative to the individual weekly assignments. Instead of separate deliverables, you'll build a single evolving system where each week adds new capabilities. The final result is a production-style multi-agent application that demonstrates your understanding of modern GenAI concepts.

> **Theory & Learning**: Use the weekly README files for concepts, papers, and courses. This document only covers project deliverables.

---

## Project Vision

You will build a **multi-agent system** for a domain of your choice. The system should:
- Use multiple specialized agents that collaborate on complex tasks
- Incorporate RAG for grounding responses in external knowledge
- Support both local and cloud-based models with intelligent routing
- Include custom tools that agents can use
- Provide a clean interface with transparency into agent reasoning

**Choose your domain early** (Week 5). Examples for inspiration:
- Research Assistant (literature search, summarization, report generation)
- Data Analysis Pipeline (collection, analysis, visualization, reporting)
- Content Creation System (research, drafting, editing, optimization)
- Customer Support System (routing, FAQ, technical support, escalation)
- Personal Knowledge Manager (ingestion, organization, retrieval, synthesis)

Your domain choice will guide all subsequent work.

---

## Weekly Milestones

### Week 5: Foundation — LLM Integration & Prompt Engineering

**Goal**: Build the core LLM interaction layer and understand model differences.

**Deliverables**:
1. **Project Setup**
   - Poetry project with proper structure
   - Code quality tools configured (Black, Ruff, isort)
   - Basic project skeleton for your chosen domain

2. **Multi-LLM Client**
   - Unified interface for 2+ models (e.g. GPT-4 + GPT-5)
   - Streaming support
   - Error handling with retries (tenacity)
   - Token usage and cost tracking

3. **Prompt Management System**
   - Template system for your domain's core prompts
   - Implementation of different prompting strategies:
     - System/role prompting
     - Few-shot examples
     - Chain-of-thought
     - Structured output (JSON mode)
   - Easy switching between strategies for testing

4. **Simple Interface**
   - Streamlit/Gradio app for interacting with your system
   - Model selection and comparison view
   - Response metadata display (tokens, latency, cost)

**Week 5 Checkpoint**:
- [ ] Can query multiple LLMs through unified interface
- [ ] Cost tracking shows per-request token usage
- [ ] At least 3 prompt strategies implemented and testable
- [ ] Basic UI allows model comparison

---

### Week 6: Local Models & Intelligent Routing

**Goal**: Add local model support and implement smart model selection.

**Deliverables**:
1. **Local Model Integration**
   - Ollama (or llama.cpp) setup with at least one model
   - Same unified interface as cloud models
   - Basic benchmarking: speed vs. quality comparison

2. **Query Router**
   - Analysis component that assesses query characteristics
   - Routing logic: when to use local vs. cloud models
   - Consider: complexity, required capability, cost constraints
   - Decision logging for transparency

3. **Updated Interface**
   - Local model added to comparison view
   - Routing decisions visible to user
   - Cost savings tracking

4. **Optional: Fine-tuning Exploration**
   - External notebook (Colab/Kaggle) demonstrating LoRA
   - Small fine-tuning experiment relevant to your domain
   - Brief write-up of findings

**Week 6 Checkpoint**:
- [ ] Local model responds reliably through same interface
- [ ] Router makes reasonable decisions based on query type
- [ ] Can demonstrate cost/speed tradeoffs between models
- [ ] Routing decisions are logged and explainable

---

### Week 7: RAG System

**Goal**: Add retrieval-augmented generation for grounded responses.

**Deliverables**:
1. **Document Processing Pipeline**
   - Ingestion for your domain's document types
   - Chunking strategy (experiment with at least 2 approaches)
   - Metadata extraction

2. **Vector Database**
   - pgvector, or similar
   - Populated with relevant corpus (50-100+ documents)
   - Efficient similarity search

3. **RAG Pipeline**
   - Query → Retrieve → Generate flow
   - Context injection into prompts
   - Source citation in responses

4. **Evaluation**
   - Compare RAG vs. non-RAG responses on test queries
   - Basic retrieval quality assessment
   - Document cases where RAG helps/hurts

5. **Updated Interface**
   - Document upload/management
   - Source display with responses
   - Toggle RAG on/off for comparison

**Week 7 Checkpoint**:
- [ ] Vector DB populated with domain-relevant documents
- [ ] RAG pipeline retrieves relevant context
- [ ] Responses include proper source citations
- [ ] Can demonstrate quality improvement from RAG

---

### Week 8: Multi-Agent System

**Goal**: Orchestrate multiple specialized agents into a cohesive system.

**Deliverables**:
1. **Agent Architecture Design**
   - Define 3-5 specialized agents for your domain
   - Document each agent's role, capabilities, and tools
   - Design the collaboration/handoff patterns

2. **LangGraph Implementation**
   - Multi-node workflow with your agents
   - Shared state management
   - Conditional routing between agents
   - Human-in-the-loop checkpoint for critical decisions (if needed)

3. **Tool Integration**
   - RAG retrieval as a tool
   - Model router as a tool
   - 2+ domain-specific tools (your choice)

4. **Complete System**
   - All previous weeks' work integrated
   - End-to-end flow from user query to final response
   - Agent step visualization in UI
   - Export/save functionality for results

5. **Documentation**
   - Architecture diagram
   - Agent role descriptions
   - Setup and usage instructions
   - Demo script with example queries

**Week 8 Checkpoint**:
- [ ] Multiple agents collaborate on complex queries
- [ ] Agents use tools appropriately (RAG, routing, custom)
- [ ] UI shows agent reasoning and handoffs
- [ ] System handles diverse query types in your domain

---

## Technical Requirements

### Project Structure
```
your_project_name/
├── src/
│   ├── llm/              # LLM clients (OpenAI, Anthropic, Local)
│   ├── prompts/          # Prompt templates and management
│   ├── routing/          # Query analysis and model routing
│   ├── rag/              # Vector DB, embeddings, retrieval
│   ├── agents/           # Agent definitions and LangGraph workflows
│   ├── tools/            # Custom tools for agents
│   └── ui/               # Streamlit interface
├── data/                 # Document corpus
├── notebooks/            # (optional) Experiments, fine-tuning demos
├── tests/                # Test files
├── pyproject.toml
├── .env.example
└── README.md
```

### Core Dependencies
- `openai`, `anthropic` — LLM APIs
- `requests`, `httpx` — API communication
- `pgvector` — Vector database
- `langgraph` — Agent orchestration
- `streamlit` — Web interface
- `pydantic` — Data validation

### Code Quality
- All code formatted with Black
- Linting passes with Ruff
- Imports sorted with isort
- Type hints on public functions
- Docstrings on modules and classes

---

## Evaluation Criteria

### Per-Milestone (Weekly)
Each checkpoint should be demonstrated with:
- Working code pushed to repository
- Brief walkthrough of new functionality
- Discussion of design decisions and tradeoffs

### Final Project
| Criterion | Weight | Description |
|-----------|--------|-------------|
| **Functionality** | 30% | System works end-to-end, handles edge cases |
| **Architecture** | 25% | Clean design, appropriate agent roles, good separation |
| **Code Quality** | 20% | Readable, well-structured, passes linting |
| **Integration** | 15% | All components work together seamlessly |
| **Documentation** | 10% | Clear README, architecture docs, setup instructions |

### Demo Requirements
Final demo should include:
1. Architecture overview (5 min)
2. Live walkthrough with 3-5 diverse queries (10 min)
3. Agent reasoning visualization
4. Discussion of design decisions and lessons learned (5 min)

---

## Tips for Success

1. **Start with your domain**: Week 5 decisions shape everything. Pick something you find interesting.

2. **Build incrementally**: Each week should produce working software. Don't plan for "I'll fix it later."

3. **Keep it simple first**: Get basic versions working before adding complexity. A simple working router beats a complex broken one.

4. **Test as you go**: Create a set of test queries early and use them throughout to catch regressions.

5. **Document decisions**: Keep notes on why you chose certain approaches. Useful for final presentation and future reference.

6. **Ask questions early**: If you're stuck on architecture decisions, discuss it before implementing.
