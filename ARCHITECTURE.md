
---

# `ARCHITECTURE.md`

```md
# CodeSentinel Architecture

## Overview

CodeSentinel is a local-first AI developer tool implemented as a VS Code extension with a Python backend.

The architecture separates the editor interface from code intelligence, retrieval, and AI inference.

---

# High-Level Architecture

```text
                    VS CODE
┌──────────────────────────────────────────────┐
│                                              │
│              CodeSentinel                    │
│                                              │
│ Sidebar │ Commands │ Diagnostics │ Webview    │
│                                              │
└──────────────────────┬───────────────────────┘
                       │
                       │ HTTP / JSON
                       ▼
                 FASTAPI BACKEND
                       │
       ┌───────────────┼────────────────┐
       │               │                │
       ▼               ▼                ▼
   Indexing        Retrieval           Git
       │               │
       ▼               ▼
 Tree-sitter        Qdrant
       │               │
       ▼               ▼
      AST          Embeddings
                       │
                       ▼
                    Ollama
                       │
                       ▼
                    LLM
