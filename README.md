# Ievgen Akhrimienko — AI Automation & Solutions Engineer

Production AI products, end-to-end: LLM agents & chatbots, RAG, realtime voice AI,
API/CRM integrations, Python data pipelines, and full-stack web on Next.js / React.
Founder of **Ahrim AI Lab**.

🌐 **Live demo & portfolio:** [brokerdesk-ai.com](https://brokerdesk-ai.com)
💻 **Sanitized code samples:** [`/code-samples`](./code-samples)

> Most of my code lives in **private repositories** (client & product work).
> This repo is a curated overview with a few sanitized excerpts — happy to
> **walk through any codebase on a call** or grant read access on request.

---

## Selected projects

### 🏢 BrokerDesk AI — [brokerdesk-ai.com](https://brokerdesk-ai.com)
Full-stack AI platform for real-estate brokerages, built solo (product → infra).
- **Full-stack:** Next.js 16 / React 19 / TypeScript
- **Realtime voice agent:** OpenAI Realtime API over WebRTC — inbound/outbound personas, function calling
- **Omnichannel:** web + WhatsApp chat, lead qualification
- **Integrations:** 7-stage HubSpot pipeline, Cal.com, Telegram
- **Quality/infra:** Lighthouse 88 / A11y 100 / SEO 100, Dockerized, CI/CD
- Production-hardening: migrated OpenAI Realtime beta→GA with zero downtime; routed calls through a Vercel Edge proxy when the host blocked outbound TCP to foreign APIs
- 💻 Code sample: [`realtime-token-route.ts`](./code-samples/realtime-token-route.ts)

### 🌐 AI voice web app
Full-stack marketing site with a **live in-browser voice agent** (talk to the AI right on the page).
- Next.js 16 / React 19 / TypeScript, server-rendered, SEO-optimized
- In-browser realtime voice demo (ephemeral-token pattern), rate-limited
- Lead capture wired to Telegram + Google Sheets and an n8n callback flow
- Dockerized, deployed and maintained end-to-end

### 🎙️ Voice AI agents on Voximplant
Production voice agents on **VoxEngine + OpenAI Realtime API**.
- Inbound receptionist (answers, qualifies leads, hands off to a human)
- Outbound sales dialer (warm-base calling)
- Function calling (lead capture, callback scheduling, call end), transcript → structured lead extraction
- Voice-specific engineering: VAD tuning, barge-in handling, ASR-error robustness, voice selection
- Multilingual: Russian & English personas
- ▶ Demos: [outbound call](https://youtu.be/mHRJRCaOhxw) · [inbound receptionist (24/7)](https://youtu.be/oMa_S6Oatp8)
- 💻 Code sample: [`voximplant-voice-agent.js`](./code-samples/voximplant-voice-agent.js)

### 📚 RAG support assistant
Retrieval-augmented knowledge assistant grounded strictly in a company's own docs.
- Ingestion (documents + video transcribed via Whisper) → chunking → embeddings → vector search
- Answers grounded in the knowledge base with anti-hallucination guardrails and dialogue memory
- ~$30–50/month inference vs. a full-time human handling the same first-line load

### 🔄 End-to-end sales automation
- Python scrapers/parsers for lead collection & enrichment (dedup, validation)
- CRM sync via API (amoCRM / HubSpot)
- Orchestration in n8n → Telegram alerts + Google Sheets dashboards
- 💻 Code sample: [`llm_client.py`](./code-samples/llm_client.py)

### 🛒 Marketplace automation
- Autoload feed generation and a management system (Python) for automated classifieds listings

---

## Tech stack

| Area | Tools |
|------|-------|
| **AI / LLM** | OpenAI API, Anthropic/Claude, OpenAI Realtime, LLM agents, RAG, embeddings, vector search, prompt engineering, voice AI (STT/TTS) |
| **Automation** | n8n, Make, workflow design, CRM automation, webhooks |
| **Backend** | Python (FastAPI), Node.js, REST APIs, web scraping |
| **Full-stack** | Next.js, React, TypeScript, HTML/CSS |
| **Data / Infra** | PostgreSQL, Docker, Git, Linux, CI/CD |

---

📫 Reach out for a walkthrough, code access, or collaboration: **ievgen.akhrimienko@gmail.com**
