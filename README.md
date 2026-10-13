# 🚀 Enterprise n8n AI Automation & Workflow Suite

A collection of production-grade, scalable n8n workflows designed to eliminate manual business overhead, automate customer operations, and integrate frontier AI models (OpenAI, Claude) with vector search and backend databases.

---

## 🏗️ Architecture & Core Workflows

### 1. Autonomous AI Customer Support & RAG Agent
* **What it does:** Automatically ingests inbound client support tickets, queries a vector knowledge base (Pinecone/Supabase) via RAG, drafts context-aware responses using Claude 3.5 Sonnet, and routes complex edge cases to human agents via Slack.
* **Tech Stack:** n8n, OpenAI/Anthropic APIs, Pinecone Vector DB, Webhooks, Slack API, PostgreSQL.
* **Workflow File:** [`workflows/ai_support_rag_agent.json`](./workflows/ai_support_rag_agent.json)

### 2. Automated Lead Enrichment & Scoring Pipeline
* **What it does:** Listens to incoming webhook triggers from web forms, cleans and enriches lead data, calculates an AI-driven ICP (Ideal Customer Profile) score, and updates the CRM (HubSpot/Airtable) in real-time.
* **Tech Stack:** n8n, JavaScript Function Nodes, REST APIs, HubSpot, Airtable.
* **Workflow File:** [`workflows/lead_enrichment_pipeline.json`](./workflows/lead_enrichment_pipeline.json)

---

## 🛠️ Key Technical Highlights
* **Custom JavaScript/Python Nodes:** Uses custom data-transformation code inside n8n to handle complex JSON payloads, array manipulations, and custom error-handling loops.
* **Secure Webhooks & Authentication:** Implements HMAC signature verification and secure credential mapping.
* **Self-Hosted Infrastructure:** Designed to run reliably on Docker-deployed n8n instances with high availability and strict data privacy compliance.

---
