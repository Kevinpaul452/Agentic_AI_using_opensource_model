# Agentic Web Summarizer using LangChain and OpenRouter

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

* The agent decides which tools to call

* Tools are implemented as Python functions

* The LLM orchestrates the workflow using reasoning + tool-calling

## Tech Stack

1. LangChain – Agent framework and tool orchestration

2. OpenRouter – LLM provider

3. BeautifulSoup – Web scraping

4. Python – Core implementation

## Setup
1. Install dependencies
   ```python
   pip install langchain langchain-core langchain-community langchain-openrouter beautifulsoup4 requests
   ```
3. Set API Key
   ``` json
   import os
   os.environ["OPENROUTER_API_KEY"] = "your_api_key"
   ```
