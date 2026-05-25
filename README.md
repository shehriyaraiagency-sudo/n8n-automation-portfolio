# n8n AI Automation Portfolio — Week 1

Built in Baku, Azerbaijan as part of a 60-day AI automation agency roadmap.

## Workflows

### 1. Webhook → Groq API → HTTP Response
Basic AI endpoint. Receives POST request, queries Groq LLM, returns AI reply.
**Stack:** n8n · Groq API · llama-3.3-70b-versatile

### 2. Telegram Bot with Conversation Memory
Full Telegram bot with Supabase memory, rate limiting, error handling, and commands.
**Features:** /start · /help · /reset · typing indicator · fallback messages
**Stack:** n8n · Groq API · Telegram Bot API · Supabase

### 3. Lead Capture — Google Form
Google Form submission → owner notification → lead confirmation email.
**Stack:** n8n · Google Sheets API · Gmail API

### 4. Lead Capture — n8n Native Form
n8n hosted form → delayed confirmation email.
**Stack:** n8n · Gmail API

### 5. Existing Leads Processor
One-time workflow to process leads that existed before automation was activated.
**Stack:** n8n · Google Sheets API · Gmail API

### 6. Telegram Bot Simple
Basic Telegram bot without memory. Entry-level product.
**Stack:** n8n · Groq API · Telegram Bot API

### 7. Monthly History Cleanup
Scheduled workflow — deletes Supabase messages older than 30 days automatically.
**Stack:** n8n · Supabase

## Setup
1. Import any `.json` file into your n8n instance
2. Replace credential placeholders with your own API keys
3. Activate workflow

## Tech Stack
- n8n (self-hosted)
- Groq API (llama-3.3-70b-versatile)
- Telegram Bot API
- Google Sheets API
- Gmail API
- Supabase (PostgreSQL)

## Author
Şəhriyar Aslanov | AI Automation Specialist | Baku, Azerbaijan
