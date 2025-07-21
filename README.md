# 🧠 RAG Chatbot with Multi-Platform Integrations & Permission Control

This project is a full-stack Retrieval-Augmented Generation (RAG) system powered by **LlamaIndex**, built to ingest, query, and respond using real-time data from multiple third-party platforms — all while enforcing fine-grained user permissions.

---

## 🚀 Tech Stack

**Backend:**
- Python
- [LlamaIndex](https://www.llamaindex.ai/)
- Parato (custom app framework for orchestration)
- FastAPI (optional layer for API serving)
- Paragon (for workflow automation)

**Integrations:**
- Google Drive API
- Slack API
- Notion API
- Dropbox API
- Okta FGA (Fine-Grained Authorization)

**Data Pipeline & Infra:**
- Webhooks & Polling for sync
- Paragon Paragraph templates
- Real-time permission syncing
- RAG architecture with embedding + vector store (e.g., FAISS or Weaviate)

---

## ✨ Key Features

### 🔗 Multi-Platform Integration (Part 1)
Parato automatically ingests and syncs data from:
- **Google Drive:** including live permission data
- **Slack:** channel messages, threads, file links
- **Notion:** structured pages, blocks, and databases

The system uses LlamaIndex to embed and index this data, allowing the chatbot to respond with up-to-date and relevant context from all connected platforms.

### 🔒 Fine-Grained Permissions (Part 2)
Responses are restricted to only the data the querying user has access to:
- Google Drive and Dropbox permission trees are parsed and indexed
- Okta FGA manages unified user access across all platforms
- Access control is enforced at **query time**, in real-time

---

## 📚 Use Cases

- Secure AI knowledge assistants for enterprise teams
- Contextual search/chat over multi-platform company data
- Permission-aware internal tools for HR, Legal, or IT

---

## 🧪 Status

Actively under development. This repo is focused on core functionality for ingestion and permission control, with more advanced RAG routing and agentic behavior planned for the future.

---

## 📥 Contact

For contributions, feedback, or implementation help, reach out to **@ammaarym** on GitHub.
