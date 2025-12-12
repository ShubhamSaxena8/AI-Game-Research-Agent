## Set up instructions:

### Environment Setup
Create a `.env` file with the following API keys:
```
OPENAI_API_KEY="YOUR_KEY"
CHROMA_OPENAI_API_KEY="YOUR_KEY"
TAVILY_API_KEY="YOUR_KEY"
```

### Project Dependencies
- Python 3.11+
- ChromaDB
- OpenAI
- Tavily
- dotenv

### Directory Structure
```
project/
├── starter/
│   ├── games/           # JSON files with game data
│   ├── lib/             # Custom library implementations
│   │   ├── llm.py       # LLM abstractions
│   │   ├── messages.py  # Message handling
│   │   ├── ...
│   │   └── tooling.py   # Tool implementations
│   ├── Udaplay_01_starter_project.ipynb  # Part 1 implementation
│   └── Udaplay_02_starter_project.ipynb  # Part 2 implementation
```

## Getting Started

1. Create and activate a virtual environment
2. Install required dependencies
3. Set up your `.env` file with necessary API keys
4. Follow the notebooks in order:
   - Complete Part 1 to set up your vector database
   - Complete Part 2 to implement the AI agent

## Testing Your Implementation

After completing both parts, test your agent with questions like:
- "When was Pokémon Gold and Silver released?"
- "Which one was the first 3D platformer Mario game?"
- "Was Mortal Kombat X released for PlayStation 5?"

## Advanced Features

After completing the basic implementation, you can enhance your agent with:
- Long-term memory capabilities
- Additional tools and capabilities

## Notes
- Make sure to implement proper error handling
- Follow best practices for API key management
- Document your code thoroughly
- Test your implementation with various types of queries
