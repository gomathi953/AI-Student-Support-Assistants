# AI Student Support Assistant

**Use Case #1 — AI Agentic Project Submission**

An intelligent support assistant that answers college-related questions
by grounding responses in institutional regulations, syllabus documents,
FAQs, and notices — combining Retrieval-Augmented Generation (RAG), tool
calling, and session memory into a single conversational agent.

## Folder Structure

```
AI_Student_Support_Assistant/
├── README.md                              This file
├── requirements.txt                        Python dependencies for the backend/RAG pipeline
├── docs/
│   └── AI_Student_Support_Assistant.docx   Full project report (overview, objectives,
│                                            architecture, tech stack, results, conclusion)
└── prototype/
    └── index.html                          Interactive front-end prototype (chat UI demo)
```

## How to Run

**View the prototype (no setup needed):**
Open `prototype/index.html` directly in any web browser. It runs entirely
client-side with simulated agent responses, so no server or dependencies
are required to demo the UI/UX.

**Set up the full backend (RAG + tools + memory):**
```bash
pip install -r requirements.txt
```
Then follow the architecture described in `docs/AI_Student_Support_Assistant.docx`
to connect the retrieval pipeline, tool functions, and the Claude API.

## Project Summary

| | |
|---|---|
| **What it builds** | Answers college-related questions from regulations, syllabus, FAQs and notices |
| **Key agent capabilities** | RAG + Tools + Memory |
| **LLM / Reasoning** | Claude (Anthropic API) |
| **Retrieval** | Vector database (Chroma / FAISS / Pinecone) |
| **Interface** | Web-based chat UI |

See `docs/AI_Student_Support_Assistant.docx` for the complete report, including
problem statement, objectives, working process, evaluation metrics, and future scope.

## Try Asking (in the prototype)
- "What's the minimum attendance required?"
- "When are the semester exam fees due?"
- "What topics are in the syllabus for Data Structures unit 3?"
- "Any new notices for CSE this week?"
- "How many backlogs am I allowed to carry?"

> Note: the prototype simulates agent responses for demo purposes. It is not
> yet connected to a live LLM/RAG backend.
