# José Manuel Da Silva

**Operations leader who builds the automation himself.** Years running restaurant
operations (80+ openings, a brand scaled from €300K to almost €5M in revenue), now
building AI agents, API integrations and automated reporting in Python, n8n and
serverless JavaScript. I start from the process, not from the tool: walk it with
the people who do it, find the manual work, automate it, and check the output
against the source data before calling it done. Adoption is the deliverable, not
the tool.

> 🇪🇸 **En español.** Responsable de operaciones que construye la automatización
> él mismo: agentes de IA para WhatsApp y teléfono, servidores MCP, flujos n8n,
> integraciones con APIs (Meta, Google, Instagram) y reportes automáticos, en
> Python y JavaScript. Madrid · español nativo, inglés C1.

📍 Madrid, Spain · [LinkedIn](https://www.linkedin.com/in/jose-manuel-da-silva-gonzalez-71a6a1a9) · [umbrelia.es](https://umbrelia.es)

---

## AI agents

| Project | What it does | Stack |
|---|---|---|
| [**Umbrelia**](https://github.com/josemdasilvag-blip/umbrelia) | AI receptionist for appointment businesses on WhatsApp and phone: answers from the business's own data, books, moves and cancels appointments, hands off to a person when unsure. Multi-tenant, running on a cloud server. [Talk to it in your browser](https://josemdasilvag-blip.github.io/umbrelia/). Backend private. | Python · Claude API (tool use) · WhatsApp Cloud API · ElevenLabs · Google Calendar · Hetzner · Cloudflare |
| [**whatsapp-booking-agent**](https://github.com/josemdasilvag-blip/whatsapp-booking-agent) | Restaurant booking agent: MCP server with 7 tools plus a WhatsApp webhook. Deterministic availability engine (capacity, table-turn times, ordered alternatives); an optional LLM layer interprets free text and the code validates. **149 tests.** | Python · MCP · WhatsApp Cloud API · Claude |
| [**venue-ops-mcp**](https://github.com/josemdasilvag-blip/venue-ops-mcp) | MCP server that lets Claude query multi-site restaurant figures and detect where money leaks (discounts, comps, voids) as drift or spikes against a baseline. CI on GitHub Actions. | Python · MCP SDK · Pydantic |

## Workflow automation & integrations

| Project | What it does | Stack |
|---|---|---|
| [**n8n-pos-daily-report**](https://github.com/josemdasilvag-blip/n8n-pos-daily-report) | Daily close report: POS tickets → KPIs and control block → Telegram before the morning meeting. Importable workflow. | n8n · JavaScript · Telegram API |
| [**instagram-comment-to-dm**](https://github.com/josemdasilvag-blip/instagram-comment-to-dm) | Keyword comment → Instagram DM, replacing a Meta automation not available to EU businesses. Self-renewing token, idempotent. **In production.** | Cloudflare Workers · KV · Instagram Graph API |
| [**web-audit-engine**](https://github.com/josemdasilvag-blip/web-audit-engine) | Browser automation that audits e-commerce conversion paths and produces an evidence-backed report. **Run on 75 stores.** | Node · Playwright |

## AI for content & data

| Project | What it does | Stack |
|---|---|---|
| [**reels-editor-skill**](https://github.com/josemdasilvag-blip/reels-editor-skill) | Claude Code skill that edits talking-head videos end to end: silence cuts, word-level captions, hook, brand styling. | Claude Code · faster-whisper · ffmpeg |
| [**instagram-analytics**](https://github.com/josemdasilvag-blip/instagram-analytics) | Transcribes 103 reels, groups them by topic and compares the follower funnel per topic, to decide what to make next. | Python · Whisper · Node |

## Also running, not public

Private because they hold client or business data:

- **Automated weekly reports** for businesses (bookings, conversations, Google reviews with an improvement plan), generated as PDF and sent by WhatsApp and email on a schedule.
- **Google reviews agent**: drafts replies; positive reviews are published automatically, negative ones go to the owner for approval.
- **Email nurture pipeline**: web forms → Cloudflare Worker + D1 → MailerLite groups and drip sequences.
- **Lead generation pipeline**: Google Places data, website crawling to qualify prospects, email verification and cold-email loading.
- **Scheduled AI agents** that compile a daily funnel report from web analytics and ads data, and a daily job-market scan.

## At work

- **Restalia** (franchise network): automated the daily POS report with n8n, built
  ERP + AI performance reports that got ~80% of franchisees to adopt paid training,
  and deployed an internal assistant on Microsoft Copilot.
- **Lara Grill** (multi-unit restaurant brand): selected and rolled out the full
  stack (ERP, CRM, POS, loyalty, inventory, invoice OCR, automated review replies).

## Toolbox

**Languages:** Python · JavaScript / Node.js
**Automation:** n8n · REST APIs and webhooks · OAuth2 · cron and scheduled jobs · Playwright · Cloudflare Workers
**AI:** Claude API (tool use, structured output) · Claude Code (skills, MCP servers) · OpenAI API · RAG and LangGraph (IBM certificate) · Whisper
**APIs shipped against:** WhatsApp Cloud API · Instagram Graph API · Google Calendar · Google Business Profile · Telegram · MailerLite · ElevenLabs
**Infra:** Linux / systemd · Git · GitHub Actions

## Learning projects

- [Travel recommendations](https://github.com/josemdasilvag-blip/travel_recommendation) · JavaScript course project · [live demo](https://josemdasilvag-blip.github.io/travel_recommendation/)
- [Paradise Nursery](https://github.com/josemdasilvag-blip/e-plantShopping) · IBM React course project (fork) · [live demo](https://josemdasilvag-blip.github.io/e-plantShopping/)

<sub>Course exercises and synthetic data are labelled as such in each repository.</sub>
