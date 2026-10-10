# Awesome-Sales-AI-Assistant

# Top Sales AI & Assistant Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Revenue Intelligence, Autonomous SDRs & Self-Hosted Sales AI*
**Last updated: October 2026**

This repository tracks notable **commercial sales AI platforms** and **open-source projects** that apply artificial intelligence to sales workflows — from conversation intelligence and pipeline prediction to autonomous SDRs, personalized outreach, and real-time coaching.

**Examples** include Salesforce Sales AI, Gong, Clari Copilot, People.ai, Salesloft, Outreach, Regie.ai, Attention, Lavender, and Scratchpad (the category leaders).

**Open-source emphasis**: Sales AI is a rapidly growing open-source domain. **OpenCloser** leads as a fully local-first AI sales team with AI Strategist, Lead Researcher, Voice Caller, Coach, and Manager — all running on desktop with zero cloud dependency . **simple-sales-gpt** provides a modular Go framework for building sales conversation agents with knowledge base, conversation stages, and tool registry . **free_outbound_agent** automates prospect discovery on GitHub and Dev.to with Claude/GPT-4 personalized email generation . **ai-crm-agent** demonstrates HubSpot lead scoring with human-in-the-loop outreach drafts . **WillowAI** delivers a real-time voice SDR with speech-to-text and text-to-speech . **threadr** brings tenant-scoped conversation intelligence for chat platforms . **Debrief** offers local Whisper transcription with speaker diarization and AI analysis . This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Gong](https://www.gong.io/)**
  **The conversation intelligence market leader** — call recording, transcription, deal risk detection, and AI-powered coaching insights. **Best for enterprise revenue teams**.

- **[Clari Copilot](https://www.clari.com/)**
  **Revenue intelligence with conversation analytics** — deal inspection, forecast accuracy, and coaching. **Best for revenue operations teams**.

- **[People.ai](https://people.ai/)**
  **Revenue intelligence platform** — automatically captures sales activity, identifies deal risks, and provides pipeline analytics. **Best for enterprise sales operations**.

- **[Salesloft](https://www.salesloft.com/)**
  **Sales engagement with AI** — multi-channel cadences, conversation intelligence, and revenue intelligence. **Best for enterprise inside sales teams**.

- **[Outreach](https://www.outreach.io/)**
  **Sales engagement and revenue intelligence** — sequences, deal intelligence, and AI-powered coaching. **Best for data-driven sales organizations**.

- **[Regie.ai](https://www.regie.ai/)**
  **AI-powered sales content and outreach** — generates personalized sequences and emails at scale. **Best for teams wanting AI-generated outreach**.

- **[Attention](https://www.attention.tech/)**
  **AI-powered sales coaching** — analyzes calls, auto-fills CRM, and provides 30 post-call agents for coaching and deal scoring. **Best for modern sales organizations**.

- **[Lavender](https://www.lavender.ai/)**
  **AI email coaching** — scores emails, provides real-time suggestions, and improves reply rates. **Best for SDRs and AEs wanting better cold email**.

- **[Scratchpad](https://www.scratchpad.com/)**
  **Sales AI for pipeline management** — auto-updates CRM, provides deal insights, and reduces admin time. **Best for reps wanting less CRM data entry**.

- **[Salesforce Sales AI](https://www.salesforce.com/)**
  **Salesforce's native AI** — Einstein Copilot, predictive forecasting, and automated activity capture. **Best for Salesforce customers**.

## Open-Source GitHub Projects

### Full AI Sales Platforms

- **[OpenCloser](https://github.com/issacops/opencloser-v2)**
  **Open-source AI SDR & AI sales platform running locally on your desktop**, MIT licensed . **Five AI agents**: AI Sales Strategist (generates ICP using SPIN & Challenger frameworks), AI Lead Researcher (autonomous lead hunting with scoring and Kanban CRM), AI Caller/SDR (real-time voice agent powered by Google Gemini, OpenAI Realtime, or ElevenLabs ConvAI with built-in Twilio phone lines), AI Sales Coach (objection sparring trainer with 3 difficulty levels and 12 objection archetypes), and AI Sales Manager (post-call debrief with sentiment analysis, auto-generated follow-up emails, and call analytics dashboard) . **Local-first. Zero cloud dependency.** Works fully in demo mode with no API key — 10 realistic seed leads, simulated AI calls, and all features functioning with fallback data . **Tech stack**: Tauri, React, Rust & Gemini . **Best for privacy-conscious teams wanting a complete local AI sales team**.

- **[simple-sales-gpt](https://github.com/BOFOII/simple-sales-gpt)**
  **Modular Go package for building sales conversation agents**, MIT licensed . **One agent session per conversation** with shared knowledge base for products, promotions, and vector search . **Configurable LLM provider** — use OpenAI, Claude, or any LangChainGo-compatible model . **Configurable vector store** — Chroma, Milvus, Pinecone, or any LangChainGo-compatible store . **Tool registry** with named tools, descriptions, parameters, and handlers . **Conversation stages and interest levels** for structured sales flows . **Step-based execution** for reasoning, tool selection, tool execution, and final response generation . **Best for developers building custom sales conversation agents in Go**.

- **[free_outbound_agent](https://github.com/Dumebii/free_outbound_agent)**
  **Open-source AI-powered outbound email agent**, MIT licensed . **Finds prospects on GitHub and Dev.to** using configurable search queries (e.g., `"developer advocate" in:bio`, `"indie hacker" in:bio`) . **Writes personalized emails** with Claude or GPT-4 using configurable tone, banned words, and ICP segments . **Sends via any SMTP provider** with daily limits and configurable delays (60s for ≤50 emails/day, 90s for 51-100, 120s+ for 100+) . **Multi-step follow-up sequences** with configurable delays (2 days, 3 days, 7 days) and subject hints . **LinkedIn pipeline** — message generation and state tracking while keeping you in control of actual sending (recommended for account safety) . **Best for developers wanting autonomous prospect discovery and personalized outreach**.

### Voice & Conversation AI

- **[WillowAI](https://github.com/bhartiyaanshul/willow-ai-monorepo)**
  **Open-source real-time voice SDR**, open-source . **Real-time speech-to-text and text-to-speech** with full-duplex conversation flow . **Conversational AI agent using OpenRouter** (open-source LLMs) . **Collects and summarizes lead information** during conversations . **Text-based interface** for testing and demos with persistent chat and lead storage (localStorage) . **Robust logging and transcript review** for all interactions with graceful error handling and recovery . **Tech stack**: React frontend, FastAPI backend, Whisper/Vosk STT, Coqui/Piper/gTTS TTS . **Best for teams wanting a self-hosted voice SDR with full transcript audit**.

- **[threadr](https://github.com/carverauto/threadr)**
  **Elixir-based conversation intelligence system for tenant-scoped chat ingestion, reconstruction, QA, and operator-managed bot runtimes**, open-source . **Ingests public chat activity** from platforms such as IRC and Discord . **Normalizes into tenant-scoped events** with actors, aliases, messages, mentions, relationships, and context events (edits, deletes, reactions, presence, joins, parts) . **Analyst-facing QA, history, dossier, and graph surfaces** . **Actor-centric and conversation-grounded retrieval** with embeddings, extracted entities, facts, and dialogue acts . **Periodic conversation summaries, cluster review, and relationship recompute** . **Tech stack**: Phoenix/LiveView, Ash/AshPostgres, NATS JetStream/Broadway, PostgreSQL . **Best for teams wanting deep conversation intelligence on chat platforms**.

### CRM-Integrated Sales AI

- **[ai-crm-agent](https://github.com/charlesdc003/ai-crm-agent)**
  **AI-powered CRM outreach agent with HubSpot integration**, open-source . **Fetches contacts from HubSpot CRM** via API . **Scores each lead 1-10** based on role, seniority, and company context using LLM . **Prioritizes list** — highest scores first . **Drafts personalized outreach emails** only for leads scoring 7 or above . **Recommends nurture sequences** for lower scoring leads . **Logs everything to HubSpot** — score, reasoning, priority, and email draft as a note on each contact profile . **Human in the loop** — no emails sent without human review and approval . **Tech stack**: Python, HubSpot API, Ollama/llama3.2 . **Best for teams wanting AI-assisted lead scoring with CRM integration**.

- **[Sales-Agent](https://github.com/iamqasimali/Sales-Agent)**
  **Intelligent sales automation platform powered by Ruby on Rails and LLMs**, MIT licensed . **AI-powered lead management** with scoring and prioritization . **Real-time customer insights** . **Multi-channel automation** (Email, SMS, Calls) . **Rails Admin Dashboard** . **LLM integration** (OpenAI/Gemini) . **Scalable with Docker and CI/CD via GitHub Actions** . **Best for Rails teams wanting AI-powered sales automation**.

### Conversation Analysis & Coaching

- **[Debrief](https://github.com/michael-borck/debrief)**
  **AI-powered conversation analysis with local processing and privacy-first design**, open-source . **Audio/Video support**: MP3, WAV, MP4, AVI, MOV, M4A, WebM, OGG, and more . **Privacy-first** — transcription and speaker diarization run entirely on your machine . **Local Whisper** via faster-whisper in bundled Python sidecar — no external server, no cloud upload . **Local Speaker Diarization** via pyannote.audio 3.1 with bundled model weights (MIT/CC-BY-4.0) — no HuggingFace token needed at runtime . **AI analysis** with your choice of local Ollama or OpenAI/Anthropic/Groq/Gemini/OpenRouter . **Cross-platform**: macOS, Windows, Linux with FFmpeg bundled . **Best for privacy-critical conversation analysis and sales call review**.

- **[OpenClaw Talk Analyzer](https://www.npmjs.com/package/openclaw-talk-analyzer)**
  **AI-powered business conversation analysis**, open-source . **Multi-source analysis** — audio transcripts, chat logs, meeting recordings . **AI-powered insights** — Claude, GPT, or local LLMs . **Sentiment analysis** — emotional tone and engagement levels . **Action items extraction** — tasks, decisions, and commitments . **Speaker profiling** — individual speaking patterns and contribution metrics . **Strategy recommendations** — data-driven follow-up suggestions . **Export reports** — JSON, Markdown, or PDF . **Analysis types**: Meeting Summary, Sales Call, Customer Support, Negotiation Strategy, Sentiment Tracking . **Best for multi-source conversation analysis**.

### Additional Strong Open-Source Options

- **AI Sales Agent** — Next.js 15 chatbot, content generator, and lead finder with Ollama (local, free, no API key). Includes AI Chatbot, Content Generator (blog posts, tweets, LinkedIn posts, emails), Lead Finder (web scraping), Auto Outreach, and Admin Dashboard .
- **ShampooSalesAgent** — Minimal LLM sales agent framework supporting OpenAI, Claude, HuggingFace, Gemini, Ernie, Baichuan, Qwen, Moonshot, GLM, and Deepseek. AI销售智能体微型框架 .
- **use-agent** — Gmail cold sales classifier and auto-replier using Claude Agent SDK with OAuth, safelist domains, and vendor exemption logic .
- **nora** — Multi-tenant, self-hosted conversation intelligence for meetings with PII redaction, schema-validated output, and AI telemetry .
- **voicebench** — Open-source benchmarking tool for voice agents measuring response latency, barge-in success, and WER from the outside at the audio level .

**Frameworks for building custom sales AI solutions**: Combine **OpenCloser** for a complete local AI sales team with voice calling, coaching, and pipeline management . Use **simple-sales-gpt** for a modular Go framework to build custom sales conversation agents with knowledge base and tool registry . Deploy **free_outbound_agent** for autonomous prospect discovery and personalized multi-step outreach . Integrate **ai-crm-agent** for LLM-powered lead scoring with HubSpot CRM logging and human-in-the-loop review . Use **Debrief** for privacy-first conversation analysis with local transcription and diarization . Choose **WillowAI** for a self-hosted voice SDR with full transcript audit . Note that true enterprise sales AI with conversation intelligence at scale, automated CRM sync, and vendor-supported SLAs (Gong, Clari Copilot, People.ai) remains primarily commercial territory; open-source stacks provide strong agent frameworks, voice pipelines, and conversation analysis foundations that require integration for complete sales AI operations.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Sales AI platforms handle sensitive customer conversations and may process PII. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations (GDPR, CCPA).
- **Call recording consent laws vary by jurisdiction** — two-party consent states (California, Illinois, etc.) require explicit consent before recording. Ensure compliance before deployment.
- **Human-in-the-loop is critical for outreach** — no AI-generated email should be sent without human review. Cold outreach has real business consequences and regulatory implications .
- **License considerations**: OpenCloser uses MIT , simple-sales-gpt uses MIT , free_outbound_agent is open-source , ai-crm-agent is open-source , and Debrief is open-source . Verify licensing against your use case before committing.
- The open-source ecosystem provides strong agent frameworks, voice pipelines, and conversation analysis foundations, but **real-time AI coaching, automated CRM sync at scale, and vendor-supported SLAs** remain primarily commercial offerings.
