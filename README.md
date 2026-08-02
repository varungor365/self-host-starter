<div align="center">

# 🐳 self-host-starter

**The ultimate 1-click Docker Compose starter kit for your personal AI and automation infrastructure.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Docker Compose](https://img.shields.io/badge/Docker-Compose-blue.svg)](https://docs.docker.com/compose/)

<br/>

</div>

---

## ✨ Why this exists

If you want to build personal AI agents, run local LLMs, or build RAG pipelines, you need infrastructure. Setting up Postgres with vector support, workflow automation tools, and LLM servers manually takes hours.

**self-host-starter** gives you a production-ready local stack with a single command.

### What's included?
1. 🐘 **PostgreSQL + pgvector:** The standard database, upgraded for AI embeddings and RAG.
2. 🤖 **Ollama:** Run open-source LLMs (Llama 3, Mistral) 100% locally.
3. 🌐 **Open WebUI:** A beautiful ChatGPT-like interface for your local Ollama models.
4. ⚡ **n8n:** The ultimate open-source Zapier alternative for workflow automation.
5. 🟥 **Redis:** In-memory cache for fast agent memories or queue management.

---

## 🚀 Quickstart

### 1. Configure Environment
```bash
cp .env.example .env
# Edit .env and set your passwords!
nano .env
```

### 2. Launch the Stack
```bash
docker-compose up -d
```

### 3. Access your Apps
- **Open WebUI:** `http://localhost:3000`
- **n8n:** `http://localhost:5678`
- **Postgres:** `localhost:5432`
- **Redis:** `localhost:6379`

---

## 📥 Downloading a Model

Before using Open WebUI, you need to pull an LLM into Ollama:
```bash
docker exec -it self_host_ollama ollama run llama3
```

---

## 🤖 AI Agent Context

See [CLAUDE.md](CLAUDE.md) for contribution guidelines.

---

## 📄 License

MIT © Varun Ruhella. See [LICENSE](LICENSE) for details.
