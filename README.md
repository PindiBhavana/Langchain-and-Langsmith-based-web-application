# Langchain-and-Langsmith-based-web-application
A comprehensive Streamlit web application demonstrating end-to-end integration of Large Language Models (LLMs) using LangChain and Google Gemini. This project showcases prompt engineering, API management, and production-level LLM observability using LangSmith.

🚀 Project Overview:

This repository contains the completion of a three-part technical Generative AI assignment. The application handles direct AI interactions, enforces strict system prompt constraints, and logs all background traces (latency, token usage, inputs/outputs) to a cloud dashboard.

Key Features:

Task 1: Customer Support Assistant: 
Constrained Chat & Prompt Engineering: 

Implemented a direct Q&A interface using gemini-3.8-flash via LangChain. Successfully engineered system prompts to enforce strict output formatting (e.g., maximum 2-sentence responses) and verified the constraints via trace logs.

Task 2:  Meeting Minutes & Action-Item Generator: 

Advanced LLM Integration: Document summarization, text extraction, or context-aware chat.

Task 3: AI Helpdesk Ticket Analyzer: 

Pipeline Finalization: Memory integration, chain routing, or custom tool usage.

🛠️ Technology Stack:

Frontend: Streamlit (Python)

LLM Orchestration: LangChain

Model: Google Gemini (gemini-3.8-flash)

Observability & Tracing: LangSmith

Environment Management: python-dotenv

🔍 Observability & Debugging:

This application is fully integrated with LangSmith. When LANGCHAIN_TRACING_V2 is set to "true", every interaction within the Streamlit UI is automatically logged. This allows developers to monitor:

P50 and P99 Latency

Token usage and execution costs

Raw system prompts vs. actual model outputs

During development, this tracing capability was critical in diagnosing and resolving regional endpoint configurations and API rate-limit errors.
