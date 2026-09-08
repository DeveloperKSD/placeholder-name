
---

# `docs/PRIVACY.md`

```md
# CodeSentinel Privacy

CodeSentinel is designed around a local-first architecture.

The goal is to allow developers to use AI-assisted code intelligence without requiring their source code to be uploaded to a CodeSentinel-controlled server.

---

# Default Local Architecture

```text
Source Code
     ↓
Local Parser
     ↓
Local Embeddings
     ↓
Local Qdrant
     ↓
Local LLM
