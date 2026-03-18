# Agentic_AI_using_opensource_model
### Agentic Web Summarizer using LangChain and OpenRouter

## Overview

### This project implements an agentic AI pipeline using LangChain and OpenRouter to:

1. Fetch content from a given URL

2. Process and clean webpage text

3. Generate a structured summary using LLMs

### The system follows an agent-based workflow:
User Query → Main Agent → Web Loader Tool → Summarizer Tool → Final Output

## Architecture
User Input
   ↓
Agent (LLM)
   ↓
Tool 1: load_webpage
   ↓
Tool 2: summarize_text
   ↓
Final Summary

The agent decides which tools to call

Tools are implemented as Python functions

The LLM orchestrates the workflow using reasoning + tool-calling

⚙️ Tech Stack

LangChain – Agent framework and tool orchestration

OpenRouter – LLM provider

BeautifulSoup – Web scraping

Python – Core implementation

🚀 Features

✅ Agent-based tool execution

✅ Dynamic tool selection (ReAct-style reasoning)

✅ Web content extraction

✅ Chunk-based summarization

✅ Clean structured output

✅ Debuggable execution trace (messages)
