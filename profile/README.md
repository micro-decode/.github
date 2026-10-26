# 🚀 Micro-Decode

> **Building scalable, innovative solutions for the modern web**

Welcome to **micro-decode** — a software development organization focused on creating high-performance platforms, analytics tools, and autonomous systems that power real-world businesses.

---

## 📌 Our Projects

### 1. **SkillHub Platform** 
**Repository**: [`skillhub-platform`](https://github.com/micro-decode/skillhub-platform)  
**Status**: Active Development  
**Language**: JavaScript (React Native, Node.js)

An **on-demand skilled-services marketplace** for Bangladesh. Customers book nearby verified workers (electricians, plumbers, cleaners, handymen, etc.); workers accept jobs, navigate to locations, and get paid via bKash.

**Architecture**:
- **Backend API** — Node.js/Express, PostgreSQL, Redis, real-time Socket.io
- **Customer App** — React Native (web + iOS/Android)
- **Worker App** — React Native (web + iOS/Android)
- **Admin Panel** — React + Webpack

**Key Features**:
- Real-time job matching and notifications
- Location-based worker discovery
- Integrated payment (bKash)
- Bilingual skill taxonomy with smart search
- Admin dashboard for monitoring and moderation

[👉 Explore SkillHub →](https://github.com/micro-decode/skillhub-platform)

---

### 2. **StatPriv**
**Repositories**: [`statpriv`](https://github.com/micro-decode/statpriv) · [`statpriv-pro`](https://github.com/micro-decode/statpriv-pro) · [`statpriv-theme`](https://github.com/micro-decode/statpriv-theme) · [`statpriv-license-server`](https://github.com/micro-decode/statpriv-license-server)  
**Status**: Active Development  
**Language**: PHP (WordPress Plugin + Theme)

A **self-hosted, privacy-first WordPress & WooCommerce analytics suite** for tracking user behavior, conversions, and shop performance — all data stays in the site's own database. Built on a **freemium model**: a free core plugin, a PRO plugin for advanced analytics and enterprise integrations, a marketing/landing theme, and a self-hosted license server (WCSL-compatible, driven by WooCommerce Subscriptions).

**Features**:
- User behavior tracking
- Conversion funnel analysis
- Site performance monitoring
- REST API for integrations
- PRO features for advanced analytics
- Security-hardened with input sanitization, output escaping, and nonce verification

**Architecture**:
- PSR-4 autoloading with service container
- OOP & SOLID principles
- WPCS coding standards
- Query caching and optimized database indexes

[👉 Explore StatPriv →](https://github.com/micro-decode/statpriv)

---

### 3. **Fastautonomi** — Autonomous Execution
**Repository**: [`autonomous-execution`](https://github.com/micro-decode/autonomous-execution)  
**Status**: Active Development  
**Language**: TypeScript (Turborepo monorepo)

An **AI team for your organization**. Fastautonomi pulls tasks from your project-management tool, hands each one to a specialist AI agent running in a disposable Docker worker, opens a pull request per task, and updates the task status — with independent verification, approvals and a full audit trail.

**How It Works**:
```
PM Tool → Orchestrator → Worker (Docker + Claude Agent SDK) → Verification → GitHub PR → PM Tool (status update)
```

**Architecture**:
- **Web App** — Next.js 15 + tRPC, installable PWA, SSE realtime
- **Orchestrator** — BullMQ scheduling, fair-share container capacity, crash resume
- **Workers** — disposable Docker containers running the Claude Agent SDK (never get PM credentials, never push themselves)
- **Tool Gateway** — MCP server over streamable HTTP; every connector call checked against a per-run grant
- **Engine (v2)** — run state machine, Domain Packs, templates and verifiers
- **Data** — PostgreSQL 16 + Prisma, Redis 7, AES-256-GCM encryption for secrets at rest

**Integrations**:
- **Project Management**: Linear, Jira, Superthread, GitHub Issues, plus a native Fastautonomi board
- **Version Control**: GitHub (runtime-created GitHub App, also used for "Continue with GitHub")
- **AI**: Fastautonomi AI (Claude) — a platform service, nothing for users to connect
- **Workspace & Content**: Google Workspace (Gmail, Calendar, Drive, Sheets, Docs), WordPress, web search

**Key Features**:
- **Agent team** — a Lead that routes work to specialists (Software / Frontend / Backend / QA / DevOps Engineers, Planner, Reviewer, CTO, Product Manager, CMO, SEO, Content Writer & Editor, Operations…), each with its own skills and guardrails
- **Independent AI review** and implementation briefs before code is written
- **Task dependencies & branch rules** — stacked PRs, per-task-type base branches, never a push to the default branch
- **Domain Packs** — Engineering, Content & Marketing, Ops & Admin workflow templates with built-in verifiers
- **Scheduling & reminders** — alarm-style schedules, chained workflows, web-push and email notifications
- **Memory** — remembers past tasks, reviews and PR outcomes and hands relevant context to agents
- **3D virtual office** — see every teammate's live state, hold meetings, call coworkers (WebRTC)
- **Usage metering & budgets** per agent and per organization; strict tenant isolation

[👉 Explore Fastautonomi →](https://github.com/micro-decode/autonomous-execution)

---

### 4. **Fastautonomi Marketing Site**
**Repository**: [`fastautonomi-marketing`](https://github.com/micro-decode/fastautonomi-marketing)  
**Status**: Active Development  
**Language**: TypeScript (Next.js 15, React 19, Tailwind CSS)

The **public website for Fastautonomi** at [fastautonomi.com](https://fastautonomi.com) — landing page, features, pricing (plans and credits), checkout hand-off, thank-you and "my account" pages, plus terms and privacy. The product itself lives at `app.fastautonomi.com`.

**Highlights**:
- All copy and prices kept in typed content modules, easy to change without touching layouts
- Light / dark themes, responsive down to phone width, SEO metadata and sitemap
- Build-time configuration for the site, app, account-service and contact URLs
- Playwright journey checks (every internal link, pricing → checkout → account) and screenshot checks
- Deployed as its own Docker container behind the app's Caddy (automatic HTTPS); CI checks then auto-deploys `main`

[👉 Explore the marketing site →](https://github.com/micro-decode/fastautonomi-marketing)

---

### 5. **Fastautonomi Staff Console**
**Repository**: [`neeurn-admin`](https://github.com/micro-decode/neeurn-admin) (private)  
**Status**: Active Development  
**Language**: TypeScript (Next.js 15, React 19, Tailwind CSS)

The **internal back office for the Fastautonomi team** — one place to see how the business is doing and to look after every customer,
kept in step with the product and the website because it never keeps a copy of their data: every action goes through the product's own
private API, which checks it, carries it out and records it.

**Highlights**:
- Business dashboard — recurring revenue, sign-ups, plans, AI cost and margin
- Customers, organizations, subscriptions and billing history, with personal data masked until a staff member gives a reason to see it
- Passkey-only staff sign-in, roles (Support / Finance / Owner) and a fresh passkey check before sensitive changes
- A tamper-evident, append-only audit trail of every staff action
- Reachable only through a zero-trust gate; signed, single-use, mutually authenticated requests to the product
- Next: Stripe and PayPal payments, refunds and credit management with two-person approval

[👉 Explore the staff console →](https://github.com/micro-decode/neeurn-admin)

---

### 6. **Shiksha Sutro** — Student Management
**Repository**: [`student-management`](https://github.com/micro-decode/student-management)  
**Status**: Active Development  
**Language**: PHP (Laravel 13) + TypeScript (Vue 3)

A **unified education data platform for Bangladesh**: one shared backend and one installable, offline-capable, Bangla-first PWA serving five portals — **Student, Guardian, Teacher, Institution and Government** — plus an admin console.

**Architecture**:
- **Backend** — Laravel 13 modular monolith (Identity, Registry, School Ops, Family, Reporting, Integration, Audit, Compliance), REST/JSON API with OpenAPI spec
- **Frontend** — Vue 3 + TypeScript + Vite PWA (Workbox, encrypted IndexedDB offline outbox, Bangla/English)
- **Data** — PostgreSQL, Redis (cache, queues, sessions, rate limits)
- **Deployment** — full stack in Docker Compose (nginx, PHP-FPM, queue worker, scheduler)

**Key Features**:
- Offline attendance with duplicate-free sync, marks entry and report cards with QR verification
- Admissions, transfers, promotions and bulk imports with approval workflows
- Guardian view across multiple children and schools, consent management and record corrections
- Upazila / district / national dashboards and analytics (enrolment, attendance, dropout, learning, equity, data quality)
- OTP sign-in, role switching, tamper-evident audit chain, break-glass access, de-identified exports
- Adapters for external government systems (synthetic fixtures only — all demo data is invented)

[👉 Explore Shiksha Sutro →](https://github.com/micro-decode/student-management)

---

## 🎯 What We Build

We specialize in:

✅ **Marketplace Platforms** — Real-time, scalable services on-demand  
✅ **WordPress Ecosystems** — High-performance analytics and integrations  
✅ **AI-Driven Automation** — Autonomous AI agent teams and task orchestration  
✅ **EdTech & Public-Sector Data** — Offline-first, bilingual education platforms  
✅ **Full-Stack Solutions** — From backend APIs to mobile apps and dashboards  
✅ **Cloud-Native Architecture** — Docker, Redis, PostgreSQL, microservices  
✅ **Secure Back Offices** — Passkeys, zero-trust access, tamper-evident audit trails  

---

## 🛠 Tech Stack

| Area | Tech |
|------|------|
| **Frontend** | React, React Native, Next.js, Vue 3, Tailwind CSS, three.js |
| **Backend** | Node.js/Express, TypeScript, PHP (Laravel, WordPress) |
| **Database** | PostgreSQL, Redis |
| **DevOps** | Docker, Docker Compose, Caddy, GitHub Actions, Turborepo |
| **Task Queue** | BullMQ, Laravel Queues |
| **APIs** | REST, tRPC, Socket.io, GraphQL, MCP |
| **Auth** | Auth.js, JWT, OAuth |
| **AI/ML** | Anthropic Claude API, Claude Agent SDK |

---

## 🤝 Contributing

We welcome contributions! Each repository has its own contribution guidelines. Start by:

1. Checking the specific repo's `README.md` for setup instructions
2. Reading any `CLAUDE.md` or architectural documentation
3. Opening an issue or discussion for feature requests
4. Submitting a pull request with your improvements

---

## 📖 Documentation

Each repository includes detailed documentation:

- **SkillHub**: Local development setup, seed data, API docs
- **StatPriv**: PHP architecture, plugin/theme structure, freemium design, licensing server
- **Fastautonomi**: Setup guide, operations runbook, specs, architecture decisions
- **Fastautonomi Marketing**: Content, pricing, deploy and browser-check guide
- **Fastautonomi Staff Console**: Architecture, security controls and self-review, deploy guide
- **Shiksha Sutro**: Docker setup, requirement traceability, runbook, OpenAPI spec, analytics plan

---

## 🔐 Security

We take security seriously:

- All user input is sanitized and validated
- Sensitive credentials are encrypted at rest
- APIs use proper authentication and authorization
- No secrets are committed to repositories
- Regular code reviews and security audits

---

## 📊 Organization Stats

- **9 Active Repositories** across 5 products
- **Multiple Production Services**
- **Focus**: Real-world business solutions

---

## 📧 Contact & Support

For questions about our projects:

- Open an **Issue** on the specific repository
- Check the repository's documentation files
- Review architecture decision logs in `docs/` folders

---

## 📄 License

Please refer to individual repositories for their specific licenses.

---

<div align="center">

**Built with ❤️ by the Micro-Decode Team**

[GitHub Organization](https://github.com/micro-decode) · [SkillHub](https://github.com/micro-decode/skillhub-platform) · [StatPriv](https://github.com/micro-decode/statpriv) · [Fastautonomi](https://github.com/micro-decode/autonomous-execution) · [fastautonomi.com](https://github.com/micro-decode/fastautonomi-marketing) · [Staff Console](https://github.com/micro-decode/neeurn-admin) · [Shiksha Sutro](https://github.com/micro-decode/student-management)

</div>
