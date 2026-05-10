# Intro to AI Agents with LangChain, LangGraph, and Groq

This repository contains a Jupyter Notebook demonstrating the fundamentals of building and interacting with AI agents. By leveraging the blazing-fast inference of Groq and the orchestration capabilities of LangChain and LangGraph, this project walks through basic Large Language Model (LLM) generation, custom tool creation, and web-search integration.

## 🚀 Overview

The notebook (`AiAgents.ipynb`) serves as a practical, hands-on guide to understanding how AI agents "think" and act. It transitions from simple prompt responses to multi-step reasoning using the ReAct (Reasoning and Acting) framework.

### Key Concepts Covered:
* **Basic LLM Interaction:** Initializing and querying `llama-3.3-70b-versatile` via the `ChatGroq` API.
* **Custom Tool Creation:** Using LangChain's `@tool` decorator to build custom mathematical functions (`multiply`, `divide`) that the LLM can invoke.
* **ReAct Agents:** Using LangGraph's `create_react_agent` to build an agent capable of chaining multiple tools to solve complex, multi-step queries.
* **Overcoming Knowledge Cutoffs:** Demonstrating the limitations of static LLM knowledge (e.g., asking about future events) and solving it by equipping the agent with the `DuckDuckGoSearchRun` tool for real-time web browsing.

## 🛠️ Tech Stack
* **[LangChain](https://python.langchain.com/):** For LLM wrapping and tool management.
* **[LangGraph](https://langchain-ai.github.io/langgraph/):** For creating the agentic reasoning loop.
* **[Groq](https://groq.com/):** For high-speed LLM inference.
* **[DuckDuckGo Search](https://pypi.org/project/duckduckgo-search/):** For live web retrieval.

## 📦 Prerequisites and Setup

To run this notebook, you will need:
1.  Python 3.x
2.  A [Groq API Key](https://console.groq.com/keys).

### Installation

If running locally (outside of Google Colab), install the required dependencies:

```bash
pip install langchain langchain-groq langgraph duckduckgo-search
