# AI-Game-Research-Agent
AI-powered research agent for the video game domain. It combines an offline RAG system over curated game data with web search to answer detailed questions about games, platforms, releases, and more.

## Overview

The project has two main parts:

1. **Offline RAG with ChromaDB**  
   - Builds a vector store over JSON game data with fields like name, platform, genre, publisher, description, and year of release.  
   - Supports fast semantic retrieval of relevant games for a query.

2. **AI Agent with Tools**  
   - Uses an LLM plus tools to:
     - Query the local vector DB (`retrieve_game`).  
     - Evaluate retrieval quality (`evaluate_retrieval`).  
     - Call web search when local data is insufficient (`game_web_search`).  
   - Maintains conversation state and returns structured answers.

## Tech Stack

- Python 3.11+  
- ChromaDB (vector database)  
- OpenAI (LLM)  
- Tavily (web search)  
- dotenv for environment management  

## Getting Started

- Create a virtual environment and install dependencies.  
- Add API keys to a `.env` file (`OPENAI_API_KEY`, `CHROMA_OPENAI_API_KEY`, `TAVILY_API_KEY`).  
- Run Part 1 to build the vector DB, then Part 2 to enable the full agent.

## Example Questions

- When was a specific game released?  
- Which platform a game launched on?  
- Whether a given title was released for a specific console.

UdaPlay demonstrates how to combine RAG, tools, and conversational state to build a practical domain-specific research agent.
