# YouTube RAG Bot — AI-Powered YouTube Video Q&A

An AI-powered application that enables users to ask questions about YouTube videos and receive timestamp-grounded answers using Retrieval-Augmented Generation (RAG), hybrid search, and Large Language Models (LLMs).

## Features

- **YouTube Transcript Extraction:** Extracts video transcripts with timestamps.
- **Hybrid Search:** Combines BM25 keyword search with semantic vector search.
- **Query Expansion:** Rewrites user queries to improve information retrieval.
- **Cross-Encoder Reranking:** Reranks retrieved passages to improve relevance.
- **Timestamp-Grounded Answers:** Generates answers linked to specific moments in the video.
- **Local LLM Inference:** Uses Ollama for local language model inference.
- **RAG Evaluation:** Uses RAGAS to evaluate faithfulness and answer relevance.
- **Chrome Extension:** Enables users to interact with video content directly in YouTube.

## Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Python |
| Backend API | FastAPI |
| RAG Framework | LangChain |
| Large Language Model | Ollama (Phi-3) |
| Embeddings | Hugging Face |
| Vector Database | Qdrant |
| Keyword Search | BM25 |
| Reranking | Cross-Encoder |
| Evaluation | RAGAS |
| Observability | LangSmith |

## Architecture

1. Extract transcripts from YouTube videos.
2. Split transcripts into timestamp-aware text chunks.
3. Generate vector embeddings and store them in Qdrant.
4. Rewrite and expand user queries.
5. Retrieve relevant chunks using hybrid keyword and semantic search.
6. Rerank retrieved chunks using a cross-encoder.
7. Generate answers grounded in the retrieved context.
8. Return answers with timestamps for verification.

## Use Cases

- Summarizing educational videos.
- Asking questions about technical tutorials.
- Finding specific information in lengthy videos.
- Creating searchable knowledge bases from video content.

## Learning Outcomes

- Retrieval-Augmented Generation (RAG)
- Prompt engineering and query rewriting
- Semantic search and vector embeddings
- Information retrieval and reranking
- LLM evaluation and observability
- API development using FastAPI
