# Automated AI News Digest Pipeline (n8n)

An end-to-end workflow automation built with **n8n** that fetches the latest AI news articles, summarizes them using an LLM, and delivers a clean daily email digest via the **Gmail API**.

## How It Works
1. **Trigger & Fetch:** Retrieves recent AI news articles via RSS / HTTP Request.
2. **AI Summarization:** Uses prompt engineering to format headlines in ALL CAPS and generate concise 2–3 sentence summaries.
3. **Email Delivery:** Sends the formatted newsletter automatically using Google Cloud OAuth 2.0 and Gmail.

## Setup & Usage
1. Download `ai-news-digest-workflow.json` from this repository.
2. In n8n, open a new workflow, click `...` → **Import from File**, and select the JSON file.
3. Connect your own LLM API key and Google Cloud OAuth 2.0 credentials for Gmail.
4. Click **Execute Workflow** or toggle **Active** to run on a schedule.
