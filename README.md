# Awesome-No-Code-Conversational-Bot-Builder

# Awesome No-Code Conversational Bot Builder

> A curated list of top No-Code Conversational Bot Builder platforms — both SaaS/Hosted commercial solutions and open-source alternatives for visually designing, deploying, and managing chatbots across messaging channels.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [ManyChat](#manychat)
  - [Voiceflow](#voiceflow)
  - [Ada](#ada)
  - [Yellow.ai](#yellowai)
  - [Kore.ai](#koreai)
  - [Chatfuel](#chatfuel)
- [Open-Source Software](#-open-source-software)
  - [Tiledesk Design Studio](#tiledesk-design-studio)
  - [ZernFlow](#zernflow)
  - [ChatbotX](#chatbotx)
  - [BrightBean Chat](#brightbean-chat)
  - [LangBot](#langbot)
  - [Flowise](#flowise)
  - [HeHo](#heho)
  - [InstaAuto](#instaauto)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted No-Code Conversational Bot Builder platforms. These are not open-source but are included as reference points for feature comparison.

| Platform | Type | Pricing (Starting Tier) | Free Tier Limits |
|---|---|---|---|
| **ManyChat** | Visual chatbot builder for social messaging | $15/month ($180/year billed annually) or $15/month for Pro up to 500 contacts | Free forever plan: Capped at 25 Active Contacts/month, up to 2 social channels (Instagram, Facebook Messenger, TikTok, or Telegram), 1 team seat, and max 4 live automations. |
| **Voiceflow** | Conversational design and prototyping platform | $60/month (billed annually at $50/month) for Pro plan | Free forever tier: 100 one-time non-renewing AI credits sandbox, 2 agents, 50 knowledge base data sources, and 1 editor seat. |
| **Ada** | AI-powered customer service automation | $30,000/year (billed annually, ~$2,500/month starting enterprise tier) | No free forever plan; 14-day guided proof-of-concept / pilot evaluation with custom interaction limits upon sales qualification. |
| **Yellow.ai** | Enterprise conversational AI platform | $10,000/year (~$833/month starting base enterprise tier) | Free forever plan: 1 AI Agent, 2 human agent seats, up to 500 free chat sessions/month (additional usage at $0.99/session). |
| **Kore.ai** | Enterprise conversational AI with agent platform | $50/month (Community/Starter tier; enterprise custom setups from $50,000/year) | Free forever developer sandbox: Up to 5,000 requests/month, 1 bot builder workspace, and basic NLP sandbox testing. |
| **Chatfuel** | No-code chatbot builder for messaging platforms | $18/month (billed annually at $216/year) or $20/month for Business plan | 7-day free trial with $20 bundled AI credit allowance, unlimited active contacts, and access to core visual flow building features (no free forever plan). |

---

## 🟩 Open-Source Software

Self-hosted, community-driven No-Code Conversational Bot Builder tools. The open-source ecosystem spans **visual graph-based designers**, **ManyChat alternatives for social channels**, **LLM-native bot platforms**, and **database-connected AI builders**.

### Tiledesk Design Studio
**Stack:** TypeScript / Node.js | **License:** Open Source (GitHub)
Tiledesk Design Studio is an open-source visual, no-code designer where LLM/GPT AI meets a flexible **graph-based approach** for creating conversations and automations, explicitly positioned as a **Voiceflow and Botpress alternative** [citation:15]. Key features include drag-and-drop design with AI-assisted suggestions, support for chatbots, voice assistants, and other interactive experiences [citation:15]. The broader Tiledesk platform is a full-stack open-source live chat with built-in chatbots, written in Node.js and Angular [citation:8]. The Design Studio has 453 GitHub stars and 95 forks, with active development (last push September 2026) [citation:15]. **Note:** The Tiledesk server repository shows limited code review activity (0/30 approved changesets) and no SAST or security policy detected, so production hardening should be evaluated carefully [citation:4].
**Best for:** Teams wanting a visual graph-based chatbot designer with LLM integration and human handoff, accepting a newer project than ManyChat or Voiceflow.

### ZernFlow
**Stack:** Next.js / Supabase | **License:** Open Source (GitHub)
ZernFlow is an open-source **ManyChat alternative** with a visual flow builder supporting Instagram, Facebook, WhatsApp, Telegram, Twitter/X, Bluesky, and Reddit [citation:1]. Key features include:
- **Visual Flow Builder** with 15+ node types
- **AI Response Node** via OpenAI, Anthropic, or Google (Vercel AI SDK)
- **Live Chat Inbox** with human takeover and conversation assignment
- **Contact CRM** with tags, custom fields, and segments
- **Broadcasting and Sequences** for drip campaigns
- **Comment-to-DM** automation
- **A/B Testing** and **Webhooks & HTTP** for external API integration

Deploys via Vercel with Supabase (PostgreSQL + Auth) and requires a Zernio API key for OAuth and cross-platform messaging [citation:1]. **Important limitation:** WhatsApp needs a Business Account, and Meta only accepts free-form messages within 24 hours of the contact's last message—broadcasts and delayed sequence steps can be rejected outside that window [citation:1].
**Best for:** Teams wanting a ManyChat-style visual flow builder for social media automation with AI responses, accepting the Zernio dependency and WhatsApp messaging constraints.

### ChatbotX
**Stack:** Node.js / TypeScript / Next.js / PostgreSQL / Redis | **License:** Open Source (GitHub)
ChatbotX is an open-source **ManyChat alternative built for AI**, with omnichannel marketing across WhatsApp, TikTok, Facebook, Instagram, Telegram, Zalo, Email, API, and Webchat [citation:11]. Key features include:
- **Visual Flow Builder** with 15+ node types
- **AI Agents** via OpenAI, Claude, Gemini, DeepSeek, OpenRouter, NVIDIA NIM, and Local LLMs
- **Live Chat Inbox** with human takeover
- **Contact CRM**, Broadcasting, Sequences, Team Management
- **Comment Automation** (auto-reply, like, hide) on Messenger, Instagram, Threads, and TikTok
- **A/B Testing, Triggers, Webhooks & HTTP**
- **APIs, CLI, and MCP** for advanced agent workflows

The tech stack includes Next.js 16, React 19, Drizzle ORM with PostgreSQL and pgvector, Redis with BullMQ, and S3-compatible storage [citation:11]. A standalone `chatbotx-docker-compose` repo runs pre-built images with `docker compose up`, no local checkout required [citation:11].
**Best for:** Teams wanting a feature-dense ManyChat alternative with AI agents, omnichannel coverage, and MCP support, accepting a heavier Node.js/Redis/PostgreSQL stack.

### BrightBean Chat
**Stack:** Django / HTMX / PostgreSQL | **License:** AGPL-3.0
BrightBean Chat is an open-source, self-hostable **ManyChat alternative** with a visual flow builder, shared inbox, broadcasts, sequences, and analytics across Telegram, Instagram, Messenger, WhatsApp, SMS, and email [citation:10]. It runs on Django 5, HTMX, and PostgreSQL—**no Redis, no message broker, no aggregator** between you and the platforms. Postgres is the only datastore, serving as task queue, lock manager, and rate limiter [citation:10]. Deployment via Railway includes a Postgres database, web service, and background worker. **Critical:** Back up `SECRET_KEY` and `ENCRYPTION_KEY_SALT`—they decrypt channel credentials, and a database dump without them is unreadable [citation:10]. Webhooks require a public HTTPS domain; a deployment that is not publicly reachable can send messages but never receive them [citation:10].
**Best for:** Teams wanting a lightweight ManyChat alternative without Redis or a message broker, accepting the Django/PostgreSQL stack and the critical key backup requirement.

### LangBot
**Stack:** Python | **License:** Open Source (GitHub)
LangBot is an open-source, **production-grade, LLM-native instant messaging bot development platform** with a single codebase that reaches Discord, Telegram, Slack, LINE, KOOK, Matrix, QQ, WeChat, WeCom, Lark, DingTalk, and more [citation:2]. Key capabilities include:
- **AI Conversation & Agent** with multi-turn dialogue, tool calling, multimodal support, and streaming output
- **RAG Knowledge Base** with vector retrieval and rerank re-scoring
- **Deep Agent Platform Integration** with Dify, Coze, n8n, Langflow, and others
- **MCP Protocol** client supporting Stdio and HTTP transports
- **Web Management Panel** for visual configuration and monitoring
- **Production-grade Plugin System** with hundreds of community plugins
- **Multi-pipeline Architecture** for running different bots per scenario

It uses LiteLLM as a unified model backend, supporting OpenAI, Anthropic, DeepSeek, Gemini, Ollama, and many others [citation:2].
**Best for:** Teams wanting an LLM-native bot platform with broad IM channel coverage and RAG capabilities, accepting a Python stack and configuration complexity.

### Flowise
**Stack:** Node.js / TypeScript | **License:** Apache-2.0
Flowise is an open-source **visual LLM flow builder** with drag-and-drop components for building chatbots and agents. **Important caveats:** It defaults to SQLite, which is **not safe for concurrent writes**—production deployments must switch to PostgreSQL to avoid data corruption [citation:12]. Building from source on machines with <4 GB RAM frequently triggers heap exhaustion (workaround: `--max-old-space-size=4096`) [citation:12]. **No native loop nodes**—only If/Else branching, requiring embedded code for iteration [citation:12]. Enterprise features (RBAC, SSO, audit logging) are **paywalled behind the Enterprise tier even when self-hosted** [citation:12]. Workday's acquisition has introduced roadmap uncertainty [citation:12].
**Best for:** Teams wanting a visual LLM flow builder for prototyping, accepting the SQLite concurrency risks, loop limitations, and enterprise feature gating.

### HeHo
**Stack:** Supabase / OpenRouter | **License:** MIT
HeHo is a fully open-source, **no-code AI chatbot builder** that connects directly to your own Supabase database, with no local setup required—everything works from the web [citation:6]. Key features include:
- **Connect your own Supabase** via OAuth, with automatic table creation and Row Level Security setup
- **OpenRouter integration** for 35+ free AI models (Llama, Mistral, Gemma)
- **Fine-grained database permissions**—chatbots can read data and create entries, with explicit permission boundaries
- **Hallucination reduction** by restricting AI responses to verified database queries

API keys are encrypted at rest (AES-256), and data stays inside your Supabase [citation:6]. **Note:** The project is newer and focused on database-grounded chatbots rather than broad channel deployment.
**Best for:** Teams wanting a no-code AI chatbot grounded in their own Supabase data, accepting a narrower scope than full omnichannel platforms.

### InstaAuto
**Stack:** Next.js / Supabase | **License:** Open Source (GitHub)
InstaAuto is a free, open-source **ManyChat alternative for Instagram**, self-hosted on Vercel and Supabase free tiers, connecting via the official Instagram API [citation:5]. Features include DM keyword automation, comment-to-DM funnels, story-reply automation, and a live inbox, all with **$0/month** running costs [citation:5]. It uses official Instagram API permissions and does not scrape, mass-DM, or bypass rate limits [citation:5]. **Limitation:** Instagram-only, and requires Meta app permissions and review for production use [citation:5].
**Best for:** Instagram creators wanting a free, self-hosted DM automation tool, accepting the Instagram-only scope and Meta API requirements.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Visual Builder | Omnichannel | AI/LLM | Self-Hosted | Best For |
|----------|---------|-------|----------------|-------------|--------|-------------|----------|
| **ManyChat** | Proprietary | Cloud | ✅ | ✅ IG/FB/WhatsApp | ✅ | ❌ | Social messaging automation |
| **Voiceflow** | Proprietary | Cloud | ✅ Design-first | ✅ | ✅ | ❌ | Conversational design |
| **Tiledesk Design Studio** | Open Source | TypeScript/Node | ✅ Graph-based | ✅ Multichannel | ✅ LLM | ✅ | Voiceflow/Botpress alternative |
| **ZernFlow** | Open Source | Next.js/Supabase | ✅ 15+ nodes | ✅ 7 platforms | ✅ | ✅ | ManyChat alternative |
| **ChatbotX** | Open Source | Node.js/Postgres | ✅ 15+ nodes | ✅ Broad | ✅ AI agents | ✅ | Feature-dense ManyChat alt |
| **BrightBean Chat** | AGPL-3.0 | Django/Postgres | ✅ | ✅ Multi-channel | (Check) | ✅ | No Redis/broker ManyChat alt |
| **LangBot** | Open Source | Python | (Web panel) | ✅ 15+ IM platforms | ✅ LLM-native | ✅ | Broad IM + RAG |
| **Flowise** | Apache-2.0 | Node.js | ✅ LLM flow | (Check) | ✅ | ✅ | LLM prototyping |
| **HeHo** | MIT | Supabase | (Check) | (Check) | ✅ OpenRouter | ✅ (Web) | Database-grounded bots |
| **InstaAuto** | Open Source | Next.js/Supabase | (Check) | Instagram only | ✅ | ✅ | Free IG DM automation |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source No-Code Conversational Bot Builder tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The no-code chatbot landscape is **dominated by ManyChat alternatives** rather than direct Voiceflow or Ada equivalents. **ZernFlow** and **ChatbotX** are the most direct ManyChat replacements, both offering visual flow builders with 15+ node types and AI response capabilities—ChatbotX is the more feature-dense option with MCP support and broader omnichannel coverage [citation:1][citation:11]. **BrightBean Chat** differentiates by eliminating Redis and message brokers entirely, using Postgres as the sole datastore [citation:10]. **Tiledesk Design Studio** is the closest open-source analog to Voiceflow's graph-based design approach, with LLM integration and human handoff [citation:15]. For teams wanting LLM-native bot platforms rather than ManyChat clones, **LangBot** offers the broadest IM channel coverage (15+ platforms) with RAG and MCP support [citation:2]. **Flowise** is a capable LLM flow builder but carries significant production caveats—SQLite concurrency risks, no loop nodes, and enterprise features gated behind paid tiers even when self-hosted [citation:12].

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
