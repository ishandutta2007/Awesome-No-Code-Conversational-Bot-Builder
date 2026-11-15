# Awesome-No-Code-Conversational-Bot-Builder

# Awesome No-Code Conversational Bot Builder

> A curated list of top No-Code Conversational Bot Builder platforms — both SaaS/Hosted commercial solutions and open-source alternatives for visually designing, deploying, and managing chatbots across messaging channels.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
- [Open-Source Software](#-open-source-software)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📈 Sector Overview & Market Dynamics

The global conversational AI and bot builder market is estimated at **$13 billion to $17.6 billion** and is projected to expand beyond **$80 billion to $170 billion by the mid-2030s**, compounding at a CAGR of ~21%–28%. The sector exhibits a distinct two-layer competitive dynamic: the underlying foundation models and cloud NLP infrastructure are highly **concentrated** among Big Tech hyper-scalers (Google, Microsoft, AWS, OpenAI), whereas the application and bot builder layer remains **moderately to highly fragmented**, characterized by fierce competition across specialized vertical assistants, social media automation, customer experience (CX) tools, and agile open-source alternatives.

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted No-Code Conversational Bot Builder platforms. These are not open-source but are included as reference points for feature comparison.

| Platform | Company Size (Valuation / Revenue) | Type | Pricing (Starting Tier) | Free Tier Limits |
|---|---|---|---|---|
| **Kore.ai** | ~$1.0B valuation (~$100M+ ARR, $230M+ raised) | Enterprise conversational AI with agent platform | $50/month (Community/Starter tier; enterprise custom setups from $50,000/year) | Free forever developer sandbox: Up to 5,000 requests/month, 1 bot builder workspace, and basic NLP sandbox testing. |
| **ManyChat** | ~$700M+ valuation (~$40M–$73M ARR, $163M+ raised) | Visual chatbot builder for social messaging | $15/month ($180/year billed annually) or $15/month for Pro up to 500 contacts | Free forever plan: Capped at 25 Active Contacts/month, up to 2 social channels (Instagram, Facebook Messenger, TikTok, or Telegram), 1 team seat, and max 4 live automations. |
| **Yellow.ai** | ~$550M valuation (~$40M–$80M ARR, $102M+ raised) | Enterprise conversational AI platform | $10,000/year (~$833/month starting base enterprise tier) | Free forever plan: 1 AI Agent, 2 human agent seats, up to 500 free chat sessions/month (additional usage at $0.99/session). |
| **Ada** | ~$430M valuation (acquired by Dialpad; ~$50M–$72M ARR) | AI-powered customer service automation | $30,000/year (billed annually, ~$2,500/month starting enterprise tier) | No free forever plan; 14-day guided proof-of-concept / pilot evaluation with custom interaction limits upon sales qualification. |
| **Voiceflow** | ~$105M valuation (~$30M+ ARR, $38.5M raised) | Conversational design and prototyping platform | $60/month (billed annually at $50/month) for Pro plan | Free forever tier: 100 one-time non-renewing AI credits sandbox, 2 agents, 50 knowledge base data sources, and 1 editor seat. |
| **Chatfuel** | ~$20M–$30M est. valuation (~$4M–$8M ARR, $6.7M raised) | No-code chatbot builder for messaging platforms | $18/month (billed annually at $216/year) or $20/month for Business plan | 7-day free trial with $20 bundled AI credit allowance, unlimited active contacts, and access to core visual flow building features (no free forever plan). |

---

## 🟩 Open-Source Software

Self-hosted, community-driven No-Code Conversational Bot Builder tools. The open-source ecosystem spans **visual graph-based designers**, **ManyChat alternatives for social channels**, **LLM-native bot platforms**, and **database-connected AI builders**.

### Dify [![GitHub Repo stars](https://img.shields.io/github/stars/langgenius/dify?style=social&color=white)](https://github.com/langgenius/dify/stargazers)
**Stack:** Python / Next.js / PostgreSQL / Redis | **License:** Apache-2.0
Dify is an open-source LLM application development platform that combines visual AI workflow orchestration, conversational bot creation, Agent capabilities, RAG pipelines, and model management into a single visual canvas. It provides ready-to-use web chat interfaces, API access, and integrations across messaging platforms like Slack, Discord, and WeChat.
**Best for:** Teams wanting an enterprise-grade visual AI bot and workflow builder with multi-model support, RAG, and fine-grained agent tooling.

### Langflow [![GitHub Repo stars](https://img.shields.io/github/stars/langflow-ai/langflow?style=social&color=white)](https://github.com/langflow-ai/langflow/stargazers)
**Stack:** Python / React | **License:** MIT
Langflow is a dynamic visual framework and flow builder for designing multi-agent and RAG conversational applications. Featuring a drag-and-drop canvas with pre-built components for vector databases, LLMs, prompt templates, and custom python functions, it enables rapid prototyping and visual deployment of conversational bots.
**Best for:** Developers and creators seeking a flexible Python-native visual canvas to architect complex multi-agent conversational bots.

### Flowise [![GitHub Repo stars](https://img.shields.io/github/stars/FlowiseAI/Flowise?style=social&color=white)](https://github.com/FlowiseAI/Flowise/stargazers)
**Stack:** Node.js / TypeScript | **License:** Apache-2.0
Flowise is an open-source **visual LLM flow builder** with drag-and-drop components for building chatbots and agents. **Important caveats:** It defaults to SQLite, which is **not safe for concurrent writes**—production deployments must switch to PostgreSQL to avoid data corruption. Building from source on machines with <4 GB RAM frequently triggers heap exhaustion (workaround: `--max-old-space-size=4096`). **No native loop nodes**—only If/Else branching, requiring embedded code for iteration. Enterprise features (RBAC, SSO, audit logging) are **paywalled behind the Enterprise tier even when self-hosted**.
**Best for:** Teams wanting a visual LLM flow builder for prototyping, accepting the SQLite concurrency risks, loop limitations, and enterprise feature gating.

### Chatwoot [![GitHub Repo stars](https://img.shields.io/github/stars/chatwoot/chatwoot?style=social&color=white)](https://github.com/chatwoot/chatwoot/stargazers)
**Stack:** Ruby on Rails / Vue.js / PostgreSQL / Redis | **License:** AGPL-3.0
Chatwoot is an open-source, self-hosted customer engagement and conversational support suite. It integrates deeply with live chat, WhatsApp, Facebook, Instagram, Twitter, and email, and features conversational bot automation, webhook hooks, dialogflow integrations, and interactive chatbot flows for customer communication.
**Best for:** Teams looking for a self-hosted omnichannel support hub with built-in conversational automation and human handoff.

### LangBot [![GitHub Repo stars](https://img.shields.io/github/stars/langbot-app/LangBot?style=social&color=white)](https://github.com/langbot-app/LangBot/stargazers)
**Stack:** Python | **License:** Open Source (GitHub)
LangBot is an open-source, **production-grade, LLM-native instant messaging bot development platform** with a single codebase that reaches Discord, Telegram, Slack, LINE, KOOK, Matrix, QQ, WeChat, WeCom, Lark, DingTalk, and more:
- **AI Conversation & Agent** with multi-turn dialogue, tool calling, multimodal support, and streaming output
- **RAG Knowledge Base** with vector retrieval and rerank re-scoring
- **Deep Agent Platform Integration** with Dify, Coze, n8n, Langflow, and others
- **MCP Protocol** client supporting Stdio and HTTP transports
- **Web Management Panel** for visual configuration and monitoring
- **Production-grade Plugin System** with hundreds of community plugins
- **Multi-pipeline Architecture** for running different bots per scenario

It uses LiteLLM as a unified model backend, supporting OpenAI, Anthropic, DeepSeek, Gemini, Ollama, and many others.
**Best for:** Teams wanting an LLM-native bot platform with broad IM channel coverage and RAG capabilities, accepting a Python stack and configuration complexity.

### Botpress [![GitHub Repo stars](https://img.shields.io/github/stars/botpress/botpress?style=social&color=white)](https://github.com/botpress/botpress/stargazers)
**Stack:** TypeScript / Node.js / React | **License:** AGPL-3.0 / Open Source
Botpress is an open-source conversational AI developer platform and visual flow studio for building, testing, and deploying intelligent chatbots. It provides visual dialogue management, NLU/NLP tools, omnichannel connectors (WhatsApp, Messenger, Slack, Teams, Webchat), and generative AI transitions.
**Best for:** Developers needing a modular visual chatbot builder with robust NLU capabilities and enterprise channel connectors.

### Typebot [![GitHub Repo stars](https://img.shields.io/github/stars/baptisteArno/typebot.io?style=social&color=white)](https://github.com/baptisteArno/typebot.io/stargazers)
**Stack:** TypeScript / Next.js / Prisma / PostgreSQL | **License:** AGPL-3.0
Typebot is an open-source, no-code conversational form and chatbot builder. It features an intuitive drag-and-drop block interface for visually assembling conversational flows, collecting lead qualification data, executing webhooks, and embedding bots directly into web applications or connecting via WhatsApp.
**Best for:** Marketers and builders looking for a sleek visual conversational form and lead-generation bot builder alternative to Landbot.

### ChatbotX [![GitHub Repo stars](https://img.shields.io/github/stars/ChatbotXIO/ChatbotX?style=social&color=white)](https://github.com/ChatbotXIO/ChatbotX/stargazers)
**Stack:** Node.js / TypeScript / Next.js / PostgreSQL / Redis | **License:** Open Source (GitHub)
ChatbotX is an open-source **ManyChat alternative built for AI**, with omnichannel marketing across WhatsApp, TikTok, Facebook, Instagram, Telegram, Zalo, Email, API, and Webchat:
- **Visual Flow Builder** with 15+ node types
- **AI Agents** via OpenAI, Claude, Gemini, DeepSeek, OpenRouter, NVIDIA NIM, and Local LLMs
- **Live Chat Inbox** with human takeover
- **Contact CRM**, Broadcasting, Sequences, Team Management
- **Comment Automation** (auto-reply, like, hide) on Messenger, Instagram, Threads, and TikTok
- **A/B Testing, Triggers, Webhooks & HTTP**
- **APIs, CLI, and MCP** for advanced agent workflows

The tech stack includes Next.js 16, React 19, Drizzle ORM with PostgreSQL and pgvector, Redis with BullMQ, and S3-compatible storage. A standalone `chatbotx-docker-compose` repo runs pre-built images with `docker compose up`.
**Best for:** Teams wanting a feature-dense ManyChat alternative with AI agents, omnichannel coverage, and MCP support, accepting a heavier Node.js/Redis/PostgreSQL stack.

### Tiledesk Design Studio [![GitHub Repo stars](https://img.shields.io/github/stars/Tiledesk/design-studio?style=social&color=white)](https://github.com/Tiledesk/design-studio/stargazers)
**Stack:** TypeScript / Node.js | **License:** Open Source (GitHub)
Tiledesk Design Studio is an open-source visual, no-code designer where LLM/GPT AI meets a flexible **graph-based approach** for creating conversations and automations, explicitly positioned as a **Voiceflow and Botpress alternative**. Key features include drag-and-drop design with AI-assisted suggestions, support for chatbots, voice assistants, and other interactive experiences. The broader Tiledesk platform is a full-stack open-source live chat with built-in chatbots, written in Node.js and Angular.
**Best for:** Teams wanting a visual graph-based chatbot designer with LLM integration and human handoff, accepting a newer project than ManyChat or Voiceflow.

### ZernFlow [![GitHub Repo stars](https://img.shields.io/github/stars/zernio-dev/zernflow?style=social&color=white)](https://github.com/zernio-dev/zernflow/stargazers)
**Stack:** Next.js / Supabase | **License:** Open Source (GitHub)
ZernFlow is an open-source **ManyChat alternative** with a visual flow builder supporting Instagram, Facebook, WhatsApp, Telegram, Twitter/X, Bluesky, and Reddit:
- **Visual Flow Builder** with 15+ node types
- **AI Response Node** via OpenAI, Anthropic, or Google (Vercel AI SDK)
- **Live Chat Inbox** with human takeover and conversation assignment
- **Contact CRM** with tags, custom fields, and segments
- **Broadcasting and Sequences** for drip campaigns
- **Comment-to-DM** automation
- **A/B Testing** and **Webhooks & HTTP** for external API integration

Deploys via Vercel with Supabase (PostgreSQL + Auth) and requires a Zernio API key for OAuth and cross-platform messaging. **Important limitation:** WhatsApp needs a Business Account, and Meta only accepts free-form messages within 24 hours of the contact's last message—broadcasts and delayed sequence steps can be rejected outside that window.
**Best for:** Teams wanting a ManyChat-style visual flow builder for social media automation with AI responses, accepting the Zernio dependency and WhatsApp messaging constraints.

### InstaAuto [![GitHub Repo stars](https://img.shields.io/github/stars/ayuuxh2/insta-p8?style=social&color=white)](https://github.com/ayuuxh2/insta-p8/stargazers)
**Stack:** Next.js / Supabase | **License:** Open Source (GitHub)
InstaAuto (`insta-p8`) is a free, open-source **ManyChat alternative for Instagram**, self-hosted on Vercel and Supabase free tiers, connecting via the official Instagram API. Features include DM keyword automation, comment-to-DM funnels, story-reply automation, and a live inbox, all with **$0/month** running costs. It uses official Instagram API permissions and does not scrape, mass-DM, or bypass rate limits. **Limitation:** Instagram-only, and requires Meta app permissions and review for production use.
**Best for:** Instagram creators wanting a free, self-hosted DM automation tool, accepting the Instagram-only scope and Meta API requirements.

### BrightBean Chat [![GitHub Repo stars](https://img.shields.io/github/stars/brightbeanxyz/brightbean-chat?style=social&color=white)](https://github.com/brightbeanxyz/brightbean-chat/stargazers)
**Stack:** Django / HTMX / PostgreSQL | **License:** AGPL-3.0
BrightBean Chat is an open-source, self-hostable **ManyChat alternative** with a visual flow builder, shared inbox, broadcasts, sequences, and analytics across Telegram, Instagram, Messenger, WhatsApp, SMS, and email. It runs on Django 5, HTMX, and PostgreSQL—**no Redis, no message broker, no aggregator** between you and the platforms. Postgres is the only datastore, serving as task queue, lock manager, and rate limiter. Deployment via Railway includes a Postgres database, web service, and background worker. **Critical:** Back up `SECRET_KEY` and `ENCRYPTION_KEY_SALT`—they decrypt channel credentials, and a database dump without them is unreadable. Webhooks require a public HTTPS domain; a deployment that is not publicly reachable can send messages but never receive them.
**Best for:** Teams wanting a lightweight ManyChat alternative without Redis or a message broker, accepting the Django/PostgreSQL stack and the critical key backup requirement.

### HeHo [![GitHub Repo stars](https://img.shields.io/github/stars/Sparrow-AI-Solutions/HeHo?style=social&color=white)](https://github.com/Sparrow-AI-Solutions/HeHo/stargazers)
**Stack:** Supabase / OpenRouter | **License:** MIT
HeHo is a fully open-source, **no-code AI chatbot builder** that connects directly to your own Supabase database, with no local setup required—everything works from the web:
- **Connect your own Supabase** via OAuth, with automatic table creation and Row Level Security setup
- **OpenRouter integration** for 35+ free AI models (Llama, Mistral, Gemma)
- **Fine-grained database permissions**—chatbots can read data and create entries, with explicit permission boundaries
- **Hallucination reduction** by restricting AI responses to verified database queries

API keys are encrypted at rest (AES-256), and data stays inside your Supabase. **Note:** The project is newer and focused on database-grounded chatbots rather than broad channel deployment.
**Best for:** Teams wanting a no-code AI chatbot grounded in their own Supabase data, accepting a narrower scope than full omnichannel platforms.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Visual Builder | Omnichannel | AI/LLM | Self-Hosted | Best For |
|----------|---------|-------|----------------|-------------|--------|-------------|----------|
| **Kore.ai** | Proprietary | Cloud | ✅ Enterprise Studio | ✅ 35+ channels | ✅ Multi-model / RAG | ❌ | Enterprise conversational AI |
| **ManyChat** | Proprietary | Cloud | ✅ | ✅ IG/FB/WhatsApp/TikTok | ✅ | ❌ | Social messaging automation |
| **Yellow.ai** | Proprietary | Cloud | ✅ Dynamic automation | ✅ 35+ chat & voice | ✅ Generative AI | ❌ | Enterprise voice & chat support |
| **Ada** | Proprietary | Cloud | ✅ Conversational AI | ✅ Web/Email/SMS/Social | ✅ Reasoning engine | ❌ | Customer service resolution |
| **Voiceflow** | Proprietary | Cloud | ✅ Design-first | ✅ Multichannel | ✅ | ❌ | Conversational design & prototyping |
| **Chatfuel** | Proprietary | Cloud | ✅ | ✅ IG/FB/WhatsApp | ✅ ChatGPT powered | ❌ | Social & WhatsApp chatbot builder |
| **Dify** | Apache-2.0 | Python/Next.js | ✅ Visual Canvas | ✅ Slack/Discord/Web/API | ✅ LLM-native & RAG | ✅ | Visual AI bot & workflow orchestration |
| **Langflow** | MIT | Python/React | ✅ Flow Canvas | ✅ Multi-agent / API | ✅ Multi-LLM / Vector DB | ✅ | Multi-agent conversational flows |
| **Flowise** | Apache-2.0 | Node.js | ✅ LLM flow | ✅ Web/Slack/API | ✅ Drag-and-drop | ✅ | Rapid LLM bot prototyping |
| **Chatwoot** | AGPL-3.0 | Ruby/Vue | ✅ Visual / Automation | ✅ Live chat/WA/IG/Email | ✅ AI Assist | ✅ | Omnichannel support with human handoff |
| **LangBot** | Open Source | Python | ✅ Web panel | ✅ 15+ IM platforms | ✅ LLM-native & RAG | ✅ | Broad IM coverage + RAG / MCP |
| **Botpress** | AGPL-3.0 / Open | TS/Node/React | ✅ Visual Studio | ✅ WA/Messenger/Slack/Web | ✅ NLU & Generative AI | ✅ | Modular dialogue & NLU chatbot engine |
| **Typebot** | AGPL-3.0 | TypeScript/Next | ✅ Visual Blocks | ✅ Web embed & WhatsApp | ✅ Multi-provider | ✅ | Conversational forms & lead capture |
| **ChatbotX** | Open Source | Node.js/Postgres | ✅ 15+ nodes | ✅ 9+ channels | ✅ AI agents & MCP | ✅ | Feature-dense ManyChat alternative |
| **Tiledesk Design Studio** | Open Source | TypeScript/Node | ✅ Graph-based | ✅ Multichannel | ✅ LLM & Handover | ✅ | Voiceflow/Botpress alternative |
| **ZernFlow** | Open Source | Next.js/Supabase | ✅ 15+ nodes | ✅ 7 platforms | ✅ Vercel AI SDK | ✅ | ManyChat social media alternative |
| **InstaAuto** | Open Source | Next.js/Supabase | ✅ UI Dashboard | Instagram only | ✅ AI replies | ✅ | Free Instagram DM automation |
| **BrightBean Chat** | AGPL-3.0 | Django/Postgres | ✅ Flow builder | ✅ Telegram/IG/WA/SMS | ✅ AI responses | ✅ | Lightweight ManyChat alt (no Redis) |
| **HeHo** | MIT | Supabase | ✅ Web Studio | Webchat | ✅ OpenRouter (35+ models)| ✅ (Web) | Database-grounded Supabase bots |

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
