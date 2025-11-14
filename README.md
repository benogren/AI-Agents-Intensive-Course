# 5-Day AI Agents Intensive Course with Google

## What is the 5-Day AI Agents Intensive?
This 5-day online course was crafted by Google's ML researchers and engineers to help developers explore the foundations and practical applications of AI agents. You'll learn the core components – models, tools, orchestration, memory and evaluation. Finally, you'll discover how agents move beyond LLM prototypes to become production-ready systems.

Each day blends conceptual deep dives with hands-on examples, codelabs, and live discussions. By the end, you'll be ready to build, evaluate, and deploy agents that solve real-world problems.

**Official Course:** https://www.kaggle.com/learn-guide/5-day-agents

## 🚀 Quick Start

Get started in 3 simple steps:

```bash
# 1. Run the setup script
./setup.sh

# 2. Add your Google API key to .env file
# Get your key from: https://aistudio.google.com/app/api-keys

# 3. Activate the virtual environment and run
source venv/bin/activate
cd Day-1
python day_1a_prompt_to_action.py
```

📖 For detailed setup instructions, see [QUICKSTART.md](QUICKSTART.md)

## 📚 Course Content

### Day 1: AI Agent Fundamentals
**Topics:** From Prompt to Action, Multi-Agent Systems & Workflow Patterns

**Notebooks:**
- [Day 1a: From Prompt to Action](Day-1-Notebooks/day-1a-from-prompt-to-action.ipynb) - Build your first AI agent with Google ADK
- [Day 1b: Agent Architectures](Day-1-Notebooks/day-1b-agent-architectures.ipynb) - Learn multi-agent workflow patterns

**Python Scripts:**
- [day_1a_prompt_to_action.py](Day-1/day_1a_prompt_to_action.py) - Basic agent with Google Search tool
- [day_1b_agent_architectures.py](Day-1/day_1b_agent_architectures.py) - Sequential, Parallel, and Loop workflows

**Key Concepts:**
- Building your first AI agent
- Using tools (Google Search)
- LLM-based orchestration
- Sequential workflow patterns (fixed pipelines)
- Parallel workflow patterns (concurrent execution)
- Loop workflow patterns (iterative refinement)

📖 [Day 1 Full Documentation](Day-1/README.md)

### Day 2: Agent Tools & Best Practices
**Topics:** Custom Tools, MCP Integration, Long-Running Operations

**Notebooks:**
- [Day 2a: Agent Tools](Day-2-Notebooks/day-2a-agent-tools.ipynb) - Build custom function tools and use agents as tools
- [Day 2b: Tools Best Practices](Day-2-Notebooks/day-2b-agent-tools-best-practices.ipynb) - MCP integration and long-running operations

**Python Scripts:**
- [day_2a_agent_tools.py](Day-2/day_2a_agent_tools.py) - Custom function tools and agent delegation
- [day_2b_agent_tools_best_practices.py](Day-2/day_2b_agent_tools_best_practices.py) - MCP concepts and approval workflows

**Key Concepts:**
- Custom Function Tools (Python functions as agent tools)
- Agent Tools (using agents as tools for delegation)
- Built-in Code Executor for reliable calculations
- Model Context Protocol (MCP) for external service integration
- Long-Running Operations with human-in-the-loop
- Pausable and resumable workflows

📖 [Day 2 Full Documentation](Day-2/README.md)

### Day 3: Memory Management & Context Engineering
**Topics:** Sessions, Long-Term Memory, Context Compaction

**Notebooks:**
- [Day 3a: Agent Sessions](Day-3-Notebooks/day-3a-agent-sessions.ipynb) - Sessions, state management, and persistence
- [Day 3b: Agent Memory](Day-3-Notebooks/day-3b-agent-memory.ipynb) - Long-term memory and cross-session recall

**Python Scripts:**
- [day_3a_agent_sessions.py](Day-3/day_3a_agent_sessions.py) - Stateful agents with sessions and context compaction
- [day_3b_agent_memory.py](Day-3/day_3b_agent_memory.py) - Long-term memory management and automation

**Key Concepts:**
- Sessions vs Memory (short-term vs long-term)
- InMemorySessionService vs DatabaseSessionService
- Context Compaction for reducing token costs
- Session State for sharing data within conversations
- Memory Retrieval strategies (load_memory vs preload_memory)
- Automating memory storage with callbacks
- Memory Consolidation concepts

📖 [Day 3 Full Documentation](Day-3/README.md)

### Day 4: Agent Observability & Evaluation
**Topics:** Debugging, Logging, Testing, Metrics

**Notebooks:**
- [Day 4a: Agent Observability](Day-4-Notebooks/day-4a-agent-observability.ipynb) - Logs, traces, metrics, and debugging
- [Day 4b: Agent Evaluation](Day-4-Notebooks/day-4b-agent-evaluation.ipynb) - Testing, regression detection, and quality assurance

**Python Scripts:**
- [day_4a_agent_observability.py](Day-4/day_4a_agent_observability.py) - Debugging with logs and custom plugins
- [day_4b_agent_evaluation.py](Day-4/day_4b_agent_evaluation.py) - Systematic evaluation and testing

**Key Concepts:**
- Observability pillars (logs, traces, metrics)
- ADK web UI for interactive debugging
- LoggingPlugin for production monitoring
- Custom plugins and callbacks
- Test case creation and management
- Evaluation metrics (response_match_score, tool_trajectory_avg_score)
- CLI evaluation with `adk eval` command
- User simulation for dynamic testing

📖 [Day 4 Full Documentation](Day-4/README.md)

### Day 5: Agent2Agent Communication & Production Deployment
**Topics:** A2A Protocol, Remote Agents, Production Hosting

**Notebooks:**
- [Day 5a: Agent2Agent Communication](Day-5-Notebooks/day-5a-agent2agent-communication.ipynb) - A2A protocol and cross-organization agents
- [Day 5b: Agent Deployment](Day-5-Notebooks/day-5b-agent-deployment.ipynb) - Deploying to production with Vertex AI

**Python Scripts:**
- [day_5a_agent2agent_communication.py](Day-5/day_5a_agent2agent_communication.py) - A2A protocol and remote agent integration
- [day_5b_agent_deployment.py](Day-5/day_5b_agent_deployment.py) - Production deployment guide

**Key Concepts:**
- A2A Protocol for agent-to-agent communication
- Exposing agents with to_a2a() and agent cards
- Consuming remote agents with RemoteA2aAgent
- Cross-framework, cross-language, cross-organization patterns
- Deploying to Vertex AI Agent Engine
- Production architecture and configuration
- Vertex AI Memory Bank for long-term memory
- Cost management and cleanup strategies

📖 [Day 5 Full Documentation](Day-5/README.md)

## 🛠️ Project Structure

```
AI-Agents-Intensive-Course/
├── .env                          # Your API keys (not committed to git)
├── .env.example                  # Template for .env file
├── .gitignore                    # Protects sensitive files
├── requirements.txt              # Python dependencies
├── setup.sh                      # Automated setup script
├── QUICKSTART.md                 # Quick start guide
│
├── Day-1/                        # Day 1 Python scripts
│   ├── README.md                 # Day 1 documentation
│   ├── day_1a_prompt_to_action.py
│   └── day_1b_agent_architectures.py
│
├── Day-1-Notebooks/              # Day 1 Jupyter notebooks
│   ├── day-1a-from-prompt-to-action.ipynb
│   └── day-1b-agent-architectures.ipynb
│
├── Day-2/                        # Day 2 Python scripts
│   ├── README.md                 # Day 2 documentation
│   ├── day_2a_agent_tools.py
│   └── day_2b_agent_tools_best_practices.py
│
├── Day-2-Notebooks/              # Day 2 Jupyter notebooks
│   ├── day-2a-agent-tools.ipynb
│   └── day-2b-agent-tools-best-practices.ipynb
│
├── Day-3/                        # Day 3 Python scripts
│   ├── README.md                 # Day 3 documentation
│   ├── day_3a_agent_sessions.py
│   └── day_3b_agent_memory.py
│
├── Day-3-Notebooks/              # Day 3 Jupyter notebooks
│   ├── day-3a-agent-sessions.ipynb
│   └── day-3b-agent-memory.ipynb
│
├── Day-4/                        # Day 4 Python scripts
│   ├── README.md                 # Day 4 documentation
│   ├── day_4a_agent_observability.py
│   └── day_4b_agent_evaluation.py
│
├── Day-4-Notebooks/              # Day 4 Jupyter notebooks
│   ├── day-4a-agent-observability.ipynb
│   └── day-4b-agent-evaluation.ipynb
│
├── Day-5/                        # Day 5 Python scripts
│   ├── README.md                 # Day 5 documentation
│   ├── day_5a_agent2agent_communication.py
│   └── day_5b_agent_deployment.py
│
└── Day-5-Notebooks/              # Day 5 Jupyter notebooks
    ├── day-5a-agent2agent-communication.ipynb
    └── day-5b-agent-deployment.ipynb
```

## 🔧 Technologies Used

- **[Google ADK](https://google.github.io/adk-docs/)** - Agent Development Kit for building AI agents
- **[Gemini API](https://ai.google.dev/gemini-api/docs)** - Google's powerful LLM
- **Python 3.14+** - Programming language
- **python-dotenv** - Environment variable management

## 📖 Learning Resources

- [ADK Documentation](https://google.github.io/adk-docs/)
- [ADK Quickstart for Python](https://google.github.io/adk-docs/get-started/python/)
- [Gemini API Documentation](https://ai.google.dev/gemini-api/docs)
- [Kaggle 5-Day Agents Course](https://www.kaggle.com/learn-guide/5-day-agents)

## 🔐 Security Note

Your API keys are stored in the `.env` file, which is protected by `.gitignore` and will **never** be committed to version control. Always keep your API keys private!

## 💡 Tips

- Always activate the virtual environment before running scripts: `source venv/bin/activate`
- Look for `(venv)` in your terminal prompt to confirm the environment is active
- Use `deactivate` when you're done working
- Each day's folder has its own detailed README with specific instructions

## 🤝 Contributing

Feel free to enhance these scripts or add your own examples! Just make sure to:
1. Never commit your `.env` file
2. Test your changes before committing
3. Update documentation as needed

## 📝 License

This project follows the course materials which are licensed under Apache License 2.0.

---

**Happy Learning! 🎓**