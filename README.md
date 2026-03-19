# CraftAI — Open Source AI Chatbot Builder

> Build AI chatbots for your website. No PhD required. No credit card to start.

[![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
[![Python 3.12+](https://img.shields.io/badge/Python-3.12+-blue.svg)](https://www.python.org/downloads/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115+-green.svg)](https://fastapi.tiangolo.com/)

CraftAI is an open-source AI chatbot builder that lets you create, deploy, and manage AI-powered chatbots without writing AI code. Drop one script tag on your site and you're live.

---

## 🚀 Quick Start

### 1. Sign up at [craftai.hanatra.com](https://craftai.hanatra.com)

Get your API key in seconds. No credit card required.

### 2. Create a chatbot

```bash
curl -X POST https://api.craftai.hanatra.com/api/chatbots \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "name": "Support Bot",
    "instructions": "You are a helpful customer support agent for Acme Corp."
  }'
```

### 3. Embed on your site

```html
<script src="https://craftai.hanatra.com/embed.js" data-chatbot-id="YOUR_CHATBOT_ID"></script>
```

That's it. Your chatbot is live.

---

## ✨ Features

- **No-code chatbot builder** — visual dashboard, no AI expertise needed
- **Contextual memory** — chatbots remember conversation history
- **RAG-ready** — connect to your documents, PDFs, knowledge bases
- **Multi-model support** — MiniMax, Claude, GPT-4, or any OpenAI-compatible API
- **Web embed** — one script tag, works on any website
- **Team collaboration** — share chatbots across your team
- **API access** — full REST API for custom integrations
- **Webhook integrations** — Slack, Discord, Notion, and more

---

## 🏗️ Tech Stack

| Layer | Technology |
|-------|-----------|
| API | FastAPI (Python 3.12+) |
| Database | PostgreSQL 16 (vector embeddings) |
| Cache | Redis 7 |
| AI Models | MiniMax, Claude, GPT-4, OpenAI-compatible |
| Auth | JWT (access + refresh tokens) |
| Storage | S3-compatible (MinIO) |
| Deployment | Linux, Docker, nginx |

---

## 🐙 For Developers

### Self-hosting

```bash
# Clone the repo
git clone https://github.com/hanatra/craftai.git
cd craftai

# Set environment variables
cp .env.example .env
# Edit .env with your API keys and database credentials

# Start with Docker Compose
docker compose up -d

# Your API is live at http://localhost:8000
# Docs at http://localhost:8000/docs
```

### Environment Variables

```env
DB_PASSWORD=your_postgres_password
JWT_SECRET=your_jwt_secret_min_32_chars
MINIMAX_API_KEY=your_minimax_key   # or OpenAI/Anthropic key
REDIS_PASSWORD=your_redis_password
```

### API Reference

Full API docs at [craftai.hanatra.com/docs](https://craftai.hanatra.com/docs).

---

## 📦 Plans

| | Free | Pro | Team |
|---|---|---|---|
| Chatbots | 3 | Unlimited | Unlimited |
| Messages/mo | 100 | 5,000 | 25,000 |
| RAG docs | — | 10 | 100 |
| Team seats | 1 | 1 | 5 |
| API access | — | ✅ | ✅ |
| | [Start free](https://craftai.hanatra.com/pricing) | $29/mo | $99/mo |

---

## 🤝 Contributing

Contributions welcome. Please read our contributing guide before submitting PRs.

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -am 'Add some feature'`
4. Push to your branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for full text.

---

## 🏢 By HANATRA

CraftAI is built and maintained by [HANATRA LIMITED](https://hanatra.com).

For support, docs, or enterprise enquiries: support@hanatra.com
