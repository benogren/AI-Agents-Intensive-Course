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

### Day 2: Coming Soon
Custom Functions, MCP Tools, and Long-Running Operations

### Day 3-5: Coming Soon
More content to be added as the course progresses

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
└── Day-2-Notebooks/              # Day 2 content (upcoming)
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