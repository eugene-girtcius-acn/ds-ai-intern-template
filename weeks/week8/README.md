## Week 8: AI Agents

### AI Agents Fundamentals
- Introduction to the agent paradigm and core componentsof agents
- ReAct (Reasoning + Acting) pattern
- Tool use and function calling with LLMs
- Planning and decomposition strategies
- Implementing memory for agents
- Model Context Protocol (MCP)

### Multi-agent systems
- Multi-agent architectures and patterns (e.g. router, supervisor)
- Agent communication
- Agent frameworks overview (LangGraph, CrewAI, AutoGen)
- Integrating RAG with agents
- Use cases for multi-agent systems
- Monitoring and observability (LangSmith, Arize, Langfuse)

### Datasets
- [HotpotQA](https://huggingface.co/datasets/hotpot_qa)

### Theory, Courses & Additional Reading

- [paper: ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/pdf/2210.03629)
- [paper: Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/pdf/2304.03442)
- [paper: Thinking Isn't an Illusion: Overcoming the Limitations of Reasoning Models via Tool Augmentations](https://arxiv.org/abs/2507.17699)
- [paper: Large Language Model based Multi-Agents: A Survey of Progress and Challenges](https://arxiv.org/abs/2402.01680)
- [paper: Automated Design of Agentic Systems](https://arxiv.org/abs/2408.08435)
- [LangGraph Documentation](https://docs.langchain.com/oss/python/langgraph/overview)
- [MCP Documentation](https://modelcontextprotocol.io/docs/getting-started/intro)
- [course: 🤗 AI Agents Course](https://huggingface.co/learn/agents-course/unit0/introduction)
- [course: AI Agents in LangGraph](https://www.deeplearning.ai/short-courses/ai-agents-in-langgraph/)
- [course: Building Agentic RAG with LlamaIndex](https://www.deeplearning.ai/short-courses/building-agentic-rag-with-llamaindex/)
- [course: Multi AI Agent Systems with crewAI](https://www.deeplearning.ai/short-courses/multi-ai-agent-systems-with-crewai/)
- [course: AI Agentic Design Patterns with AutoGen](https://www.deeplearning.ai/short-courses/ai-agentic-design-patterns-with-autogen/)

### Assignments
**Assignment 1: ReAct Agent with Custom Tools**

Specific Task: Build a reasoning agent that can use multiple tools to answer complex questions

Deliverables:

- Implement a ReAct-style agent from scratch or using LangGraph/LangChain
- Add 2-3 basic tools e.g., Web search tool, RAG retrieval tool (connect to your Week 7 RAG system), weather API
- Implement agent logging
- Simple web interface for questions

Success Criteria: Agent successfully uses appropriate tools to answer 5+ test questions

**Assignment 2: Multi-Agent System**

Specific Task: Design and build a multi-agent system for a complex task of your choice

Example systems for inspiration (do not limit yourself to these):

- **Research Assistant System**: Researcher, Fact-Checker, Writer, Editor agents collaborating on reports
- **Customer Support System**: Router, FAQ Agent, Technical Support, Escalation Handler
- **Content Creation System**: Ideation, Drafting, Editing, SEO Optimization agents
- **Data Analysis System**: Data Collector, Analyst, Visualizer, Report Generator agents

Deliverables:

- Define clear roles and responsibilities for each agent
- Implement agent communication/handoff mechanisms
- Handle supervisor/routing logic
- Add at least one capability via MCP server
- Implement agent interactions logging

Success Criteria: Multi-agent system completes assigned tasks successfully