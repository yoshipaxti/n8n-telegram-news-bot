# n8n Telegram AI News Bot

A command-driven Telegram news automation built with n8n.

This workflow ingests AI, Blockchain, and Gaming news via RSS, filters by date, removes duplicates using Google Sheets, generates AI-written captions and images, and delivers formatted posts to Telegram.

Designed for reliability, zero duplication, and editorial consistency.

---

## 🔧 Core Features

- Telegram command trigger (on-demand execution)
- Multi-category RSS ingestion
- Date-aware filtering (Yesterday + Today)
- Category tagging for downstream logic
- Google Sheets–based deduplication
- AI caption generation
- AI image generation
- Content + image merging
- Telegram image + message delivery
- Persistent state tracking

---

## 🧩 Workflow Overview

High-level flow:

Telegram Command  
→ Route by Command  
→ RSS Feeds (AI / Blockchain / Gaming)  
→ Date Filters  
→ Category Tagging  
→ Select First Item  
→ Deduplicate via Google Sheets  
→ AI Caption + AI Image  
→ Merge Content  
→ Send to Telegram  
→ Append to “Sent News” Sheet

---

## 🛠 Requirements

- n8n (self-hosted or cloud)
- Telegram Bot Token
- RSS feed URLs
- Google Sheets API credentials
- AI provider credentials (caption + image generation)

---

## 🚀 Setup

1. Import `workflow/telegram-ai-news-bot.json` into n8n
2. Configure credentials:
   - Telegram
   - Google Sheets
   - AI services
3. Create a Google Sheet with a column for processed links
4. Trigger via Telegram command


