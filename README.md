# 🎙️ Voice AI Agent ChatBot

An AI-powered voice assistant that automates tasks and talks back with wit, sarcasm, and personality - built entirely on Telegram.

## 📺 Demo Video
<img width="2730" height="1460" alt="Screenshot 2025-07-22 at 1 15 35 PM" src="https://github.com/user-attachments/assets/30ecd9a5-2e60-478d-b101-4a422af4aceb"/> 
👉 **[🎥 Watch the full demo video](https://youtu.be/NTYEfz7_zhY)**

---

## 🤖 Overview

This isn’t just another chatbot. It’s a fully modular, **AI-powered voice agent** that listens to spoken commands, performs real-world tasks like sending emails or scheduling meetings, and responds with human-like personality - including humor, sass, and contextual remarks.

---

## 🎯 What It Can Do

- 🎙️ **Voice Command Input via Telegram**
- ✉️ **Complete Email Workflow Automation**  
  - Get emails  
  - Send emails  
  - Save drafts & replies  
  - Mark read/unread  
  - Manage labels  
  - **Summarize recent emails**  
- 📅 **Calendar Scheduling**
- 📇 **Contact Lookup via Pinecone DB**
- 📝 **Generate Content for Social Media**
- 🔍 **Acts as a Search Agent**  
  - Queries Hacker News, Wikipedia, and Google using SerpAPI  
  - Fetches real-time information for responses
- 💬 **Talks Back Like a Real Human**  
  - Injects sarcasm, random one-liners, and personality in responses

---

## ⚙️ Tech Stack

| Tool                                                   | Purpose                                                      |
|--------------------------------------------------------|--------------------------------------------------------------|
| [n8n](https://n8n.io/)                                 | Workflow orchestration (no/low code)                         |
| [OpenAI GPT-4o](https://platform.openai.com)           | Language understanding, task execution, and humorous replies |
| [Pinecone](https://www.pinecone.io/)                   | Vector DB for contact memory and semantic search             |
| [Telegram Bot API](https://core.telegram.org/bots/api) | Voice command interface                                      |
| [SerpAPI](https://serpapi.com)                         | Web search tool for Google results                           |
| Wikipedia & Hacker News APIs                           | Additional search tools for context awareness                |

---

## 📂 Project Structure

```bash
Advanced_Telegram_Chatbot
├── AdvancedTelegramChatbot.json
│
├── PineconeDB/
│   ├── Mail_Agent_Pinecone.json
│   ├── Send_Mails_From_Pinecone.json
│   └── Upload_Mails_To_Pinecone.json
│
└── SubWorkflows/
    ├── CalendarAgent.json
    ├── Contacts_Agent.json
    ├── InstaPosts_SubWorkflow.json
    ├── Mails_Sub_Workflow.json
    └── telegram_search_sub_workflow.json
```
---

## 🚀 Getting Started

1. **Clone the repository**
2. **Set up your Telegram Bot**  
   - Use [@BotFather](https://t.me/BotFather) to create your bot and get the token
3. **Import the `.json` workflows into [n8n](https://n8n.io)**  
   - Import all workflows under `Advanced_Telegram_Chatbot/`, including subfolders
4. **Configure API credentials as environment variables:**

```bash
OPENAI_API_KEY=your_openai_key
PINECONE_API_KEY=your_pinecone_key
TELEGRAM_BOT_TOKEN=your_telegram_bot_token
SERPAPI_KEY=your_serpapi_key
```

5. **Deploy and start your n8n instance**
6. **Send a voice command via Telegram and watch the magic happen!** 🎙️✨

---

## 📌 Roadmap

- [ ] Integrate **RAG (Retrieval-Augmented Generation)**  
- [ ] Expand **personality profiles** (funny, formal, sarcastic, etc.)  
- [ ] Add **multi-platform support** (Slack, WhatsApp)  
- [ ] Build **Docker deployment** setup  

---

## 🤝 Let's Connect

If you're working on **voice agents**, **agentic AI**, or **automation**, feel free to fork this project, contribute, or connect with me!

**Created by:**  
👩🏽‍💻 Sushmitha Vijayakumar  
🔗 [LinkedIn](https://www.linkedin.com/in/sushmitha-vijayakumar-9b7139208)  
📝 [Medium Blog – SVEO](https://sveo-ceo.medium.com)

---
