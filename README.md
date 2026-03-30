🚀 RAG Types with LangGraph

An advanced implementation of Retrieval-Augmented Generation (RAG) systems using LangGraph, showcasing multiple modern RAG architectures:

🤖 Agentic RAG
🔄 Corrective RAG (CRAG)
🎯 Adaptive RAG

This repository demonstrates how to build stateful, production-grade RAG pipelines using graph-based orchestration.

📌 Overview

Traditional RAG pipelines are linear and limited. This project explores next-generation RAG architectures that introduce:

🧠 Multi-step reasoning via agents
🔁 Self-correction loops
⚡ Dynamic retrieval strategies

Using LangGraph, we model RAG workflows as state machines, enabling better control, observability, and modularity.

🧩 RAG Architectures Implemented
🤖 Agentic RAG

Agentic RAG leverages LLM-powered agents to dynamically decide:

When to retrieve
What tools to use
How to reason step-by-step
🔑 Features
Tool usage (search, APIs, DBs)
Multi-hop reasoning
Planning + execution agents
🔄 Flow
User Query → Planner Agent → Tool Selection → Retrieval → Reasoning → Final Answer
🔄 Corrective RAG (CRAG)

Corrective RAG introduces self-evaluation and feedback loops to improve answer quality.

Validates retrieved documents
Detects hallucinations
Re-retrieves if needed

📌 Inspired by research where systems “self-grade” retrieved context

🔄 Flow
Query → Retrieve → Generate → Evaluate → Correct → Final Answer
🎯 Adaptive RAG

Adaptive RAG dynamically selects the best strategy based on query complexity.

Simple queries → direct LLM response
Complex queries → retrieval + reasoning

📌 Combines query analysis with active/self-corrective retrieval

🔄 Flow
Query → Complexity Classifier →
    → Simple → Direct Answer
    → Complex → RAG Pipeline → Answer
    