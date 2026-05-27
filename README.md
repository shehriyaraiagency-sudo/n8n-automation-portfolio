# Week 1 — n8n AI Automation Workflows

A collection of automation workflows built with n8n, OpenAI/Groq APIs, and Google Workspace. Each workflow solves a specific business problem — replacing manual work with automated systems.

---

## Stack

| Tool | Purpose |
|------|---------|
| [n8n](https://n8n.io) | Workflow automation engine (self-hosted) |
| OpenAI API (GPT-4o) | AI language model for bot responses |
| Groq API | Fast LLM inference alternative to OpenAI |
| Telegram Bot API | Messaging channel for client-facing bots |
| Google Sheets API | Lead storage and data persistence |
| Gmail API | Automated email notifications |

---

## Workflows

---

### 1. `telegram-bot-simple.json`
**Problem it solves:** Businesses lose leads and customers because no one is available to answer Telegram messages 24/7. Staff reply slowly or miss messages entirely.

**Solution:** An AI bot that instantly responds to every Telegram message at any hour — no human required. Clients get an answer in seconds, not hours.

---

### 2. `telegram-bot-with-memory.json`
**Problem it solves:** Basic bots forget what was said in the same conversation, forcing users to repeat themselves. This makes the bot feel broken and unprofessional.

**Solution:** A Telegram bot that remembers the full conversation context. Users can ask follow-up questions naturally, just like talking to a real person.

---

### 3. `lead-capture-google-form.json`
**Problem it solves:** Businesses collect leads via Google Forms but check responses manually — sometimes hours or days later. Hot leads go cold while waiting.

**Solution:** Every form submission is instantly saved to a Google Sheet and triggers an immediate email alert to the business owner. Zero manual checking required.

---

### 4. `lead-capture-n8n-form.json`
**Problem it solves:** Same problem as above — delayed lead follow-up — but for businesses that don't use Google Forms or need a faster setup.

**Solution:** A built-in n8n form that captures leads and instantly notifies the owner via email. Deployable in minutes with no third-party form tool needed.

---

### 5. `existing-leads-processor.json`
**Problem it solves:** Businesses accumulate hundreds of unqualified leads in spreadsheets. Sales teams waste hours manually reading and scoring each one to find who is worth contacting.

**Solution:** AI automatically reads every lead, scores them by intent and budget, and flags the high-priority ones. The sales team only sees leads worth their time.

---

### 6. `daily-history-cleanup.json`
**Problem it solves:** Bots that store conversation history accumulate data indefinitely — causing slow responses, inflated API costs, and eventual system errors.

**Solution:** A scheduled workflow that automatically clears old conversation history every night. The bot stays fast, clean, and cost-efficient without manual intervention.

---

### 7. `webhook-groq-response.json`
**Problem it solves:** Businesses and developers need a fast, cheap AI response endpoint they can connect to any app, website, or tool — without building a backend from scratch.

**Solution:** A ready-made webhook endpoint powered by Groq's high-speed LLM. Send a message in, get an AI response out. Plug it into anything.

---
https://www.loom.com/share/58a55162b21a4861a91f0b143f7fc8f9
## Cost Estimates (Per Month)

| Component | Estimated Cost |
|-----------|---------------|
| VPS (n8n hosting) | $5–6/mo (DigitalOcean/Hetzner) |
| OpenAI API (GPT-4o) | $5–30/mo depending on message volume |    
| Groq API | Free tier available |
| Google APIs | Free within quota limits |

> **Always set rate limits on production bots.** A single high-traffic bot can consume $30–80/mo in API costs without limits in place.

---

## Author

Built as part of a 60-day AI Automation Agency roadmap.  
Stack: n8n · OpenAI · Groq · Telegram · Google Workspace  
Location: Baku, Azerbaijan
