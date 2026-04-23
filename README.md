# News-report-automation
 News Reporter — Automated AI Newsletter An automated daily news digest built with Make.com, OpenAI GPT-4o, DALL-E 3, and Gmail. Every morning at 9:00 AM, it fetches the latest tech headlines, rewrites them into clear summaries, generates a custom AI illustration for each story, and delivers everything straight to your inbox.

What It Does

Fetches the latest articles from a tech news RSS feed (El País Tecnología)
Sends each article to GPT-4o to generate a concise, readable summary
Sends the summary to DALL-E 3 to generate a custom image that visually represents the story
Delivers a beautifully formatted email via Gmail — automatically, every day at 9:00 AM

No manual work. No copy-pasting. Just open your inbox.

Tech Stack
Tool:
Make.com-Workflow orchestration
HTTP module-RSS feed ingestion
OpenAI GPT-4o-Article summarisation
OpenAI DALL-E 3AI- image generation
Gmail-Email delivery

 Workflow Overview
RSS Feed (El País Tech)
    ↓
HTTP Module — fetch latest articles
    ↓
GPT-4o — summarise each article in plain language
    ↓
DALL-E 3 — generate a custom image per story
    ↓
Gmail — send formatted newsletter to inbox
The workflow runs automatically on a daily schedule at 9:00 AM.

Full pipeline: HTTP → GPT-4o (summarise) → DALL-E 3 (image) → Gmail (send)

How to Replicate This

Create a free account on Make.com
Create a new Scenario
Add the following modules in order:

HTTP → GET request to any RSS feed URL
OpenAI → "Generate a completion" (GPT-4o) with a summarisation prompt
OpenAI → "Generate images" (DALL-E 3) based on the summary
Gmail → "Send an email" with the summary + image


Set the schedule trigger to Daily at your preferred time
Run once to test → then activate


Use Cases

Personal daily briefing on any topic (tech, finance, health, local news)
Internal team newsletter for companies
Content inspiration pipeline for creators
Market monitoring for business owners


Notes

This project was built as part of a Master's programme in Hyperautomation & AI Agents at EBIS Madrid
The RSS source can be swapped for any feed — the workflow is fully reusable
No coding required — 100% built with no-code tools


Author

Paula Bidian — AI & Automation Specialist
[LinkedIn](https://www.linkedin.com/in/paula-bidian-b38a7046/) · [GitHub](https://github.com/paulabidian)
