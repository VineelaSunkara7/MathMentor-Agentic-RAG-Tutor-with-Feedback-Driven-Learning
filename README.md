# MathMentor: Agentic-RAG-Tutor-with-Feedback-Driven-Learning

MathMentor is an advanced AI-powered tutoring agent built on an Agentic-RAG (Retrieval-Augmented Generation) architecture. It emulates a math professor by solving JEE-level mathematics problems with detailed, step-by-step solutions. The system uses a smart retrieval pipeline, integrates fallback web search, enforces input/output guardrails, and captures user feedback for continuous improvement.

## ✨ Key Features
### 🛡️ Guardrails with DSPy
Input Guardrail: Accepts only academic math-related questions

Output Guardrail: Filters hallucinated or irrelevant content for safety and correctness

### 📚 Knowledge Base Search (Qdrant + OpenAI Embeddings)
Retrieves similar past questions using vector similarity

Embeddings stored via llama-index for fast and persistent retrieval

Automatically routes to web search if no match found

### 🌐 Web Fallback with Tavily
When the vector DB lacks a strong match, Tavily search fetches high-quality web content

Retrieved content is passed to GPT-4o for structured explanations

### ✍️ GPT-4.1 Math Explanation Engine
Provides clear, step-by-step walkthroughs of JEE-level problems

Designed for clarity, accuracy, and instructional flow

### 👍 Human-in-the-Loop Feedback
Students can rate answers with 👍 / 👎

Feedback is stored in a local feedback.json file to inform future improvements

### 📊 Benchmarking
Tested on 50 random questions from JEEBench (HuggingFace dataset)

Current accuracy: 66%

Benchmark results saved to: benchmark/results.csv

### 💻 Streamlit-Based UI
Intuitive interface with multiple tabs

Real-time answer generation and feedback capture

### 🔁 System Architecture Overview

<img width="208" alt="image" src="https://github.com/user-attachments/assets/1451f38f-c35c-43c2-9212-3968c05eb3fb" />


