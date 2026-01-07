# Agent-Oriented RAG-Based Automated Web Scraping Intelligent Q&A System

A complete agent-oriented Retrieval-Augmented Generation (RAG) pipeline that autonomously scrapes websites using Selenium, processes text with LangChain, generates embeddings using HuggingFace models, and stores them in ChromaDB for semantic search and intelligent question answering on real-time web data.

## Project Overview

This project demonstrates an agent-oriented RAG workflow built on web-scraped data.

The system functions as a single intelligent agent that coordinates multiple tasks such as web scraping, text processing, retrieval, and answer generation to deliver grounded and context-aware responses.

The architecture follows agent-like orchestration, where each component acts as a specialized capability executed based on user intent.

## Why an Agent-Based Approach?

Traditional pipelines are static and linear.
This system behaves like an AI agent because it:

Observes user queries

Decides what data to retrieve

Uses external tools such as a scraper, vector database, and LLM

Produces responses grounded in real data

This makes it a task-driven, tool-using intelligent system, aligning with modern agent design principles.

## Features

- Agent-Oriented Web Scraping  
  Uses Selenium to dynamically fetch content from JavaScript-rendered pages as part of the agent’s data acquisition step.

- Intelligent Text Chunking  
  LangChain’s RecursiveCharacterTextSplitter enables clean and optimized text chunks for efficient retrieval.

- Semantic Understanding via Embeddings  
  HuggingFace / SentenceTransformer models generate high-quality vector representations for semantic similarity.

- Vector Memory (ChromaDB)  
  Acts as the agent’s long-term memory, enabling fast semantic search and retrieval.

- RAG-Based Reasoning  
  Retrieved context is combined with LLM reasoning to generate accurate and hallucination-reduced answers.

- Notebook-Based Execution  
  Implemented in a Jupyter Notebook with a transparent, step-by-step workflow.


## Tech Stack

Python

Selenium

LangChain

ChromaDB

HuggingFace Embeddings

LLMs (ChatGPT, LLaMA, etc.)

Jupyter Notebook

## Agent Workflow
Observation (User Query)

User submits a question

The system interprets intent

Data Acquisition (Scraping Tool)

Selenium retrieves live website content

Knowledge Processing

Clean and preprocess extracted text

Split text into chunks

Generate embeddings

Memory Storage and Retrieval

Store vectors in ChromaDB

Retrieve the most relevant chunks

Reasoning and Response

Retrieved context is passed to the LLM

LLM generates grounded, context-aware answers
