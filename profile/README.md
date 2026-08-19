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

### 2. **Growvia Analytics**
**Repository**: [`growvia-analytics`](https://github.com/micro-decode/growvia-analytics)  
**Status**: Active Development  
**Language**: PHP (WordPress Plugin)

A **high-performance WordPress analytics plugin** for tracking user behavior, conversions, and site performance. Designed with a **freemium model** for extensibility.

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

[👉 Explore Growvia Analytics →](https://github.com/micro-decode/growvia-analytics)

---

### 3. **Growvia Analytics Pro**
**Repository**: [`growvia-analytics-pro`](https://github.com/micro-decode/growvia-analytics-pro)  
**Status**: Active Development  
**Language**: PHP (WordPress Plugin)

The **PRO edition** of Growvia Analytics, extending the core plugin with advanced analytics, premium integrations, and enterprise features.

[👉 Explore Growvia Analytics Pro →](https://github.com/micro-decode/growvia-analytics-pro)

---

### 4. **Autonomous Execution (AutoFlow)**
**Repository**: [`autonomous-execution`](https://github.com/micro-decode/autonomous-execution)  
**Status**: Active Development  
**Language**: TypeScript (Full-stack)

An **intelligent task automation platform** that orchestrates coding agents to autonomously work on development tasks, open pull requests, and update project management tools.

**How It Works**:
```
PM Tool → Orchestrator → Worker (Docker + Coding Agent) → GitHub PR → PM Tool (status update)
```

**Architecture**:
- **Web Dashboard** — Next.js 15 + tRPC
- **Orchestrator** — BullMQ workers for scheduling and execution
- **Worker** — Docker container with AI coding agent
- **Database** — PostgreSQL 16 + Prisma ORM
- **Caching** — Redis 7 + BullMQ

**Supported Integrations**:
- **Project Management**: Linear, Superthread, GitHub Issues
- **AI Agent**: Anthropic Claude (API or subscription)
- **Version Control**: GitHub (with runtime-created app)

**Key Features**:
- Intelligent task assignment and scheduling
- Isolated worker environments (Docker)
- Automatic PR creation and management
- Real-time dashboard with SSE updates
- Security-hardened credential management (sealed-box encryption)

[👉 Explore Autonomous Execution →](https://github.com/micro-decode/autonomous-execution)

---

## 🎯 What We Build

We specialize in:

✅ **Marketplace Platforms** — Real-time, scalable services on-demand  
✅ **WordPress Ecosystems** — High-performance analytics and integrations  
✅ **AI-Driven Automation** — Autonomous coding agents and task orchestration  
✅ **Full-Stack Solutions** — From backend APIs to mobile apps and dashboards  
✅ **Cloud-Native Architecture** — Docker, Redis, PostgreSQL, microservices  

---

## 🛠 Tech Stack

| Area | Tech |
|------|------|
| **Frontend** | React, React Native, Next.js |
| **Backend** | Node.js/Express, PHP, TypeScript |
| **Database** | PostgreSQL, Redis |
| **DevOps** | Docker, Docker Compose |
| **Task Queue** | BullMQ |
| **APIs** | REST, tRPC, Socket.io, GraphQL |
| **Auth** | Auth.js, JWT, OAuth |
| **AI/ML** | Anthropic Claude API |

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
- **Growvia Analytics**: PHP architecture, plugin structure, freemium design
- **AutoFlow**: Setup guide, operations runbook, architecture decisions

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

- **4 Active Repositories**
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

[GitHub Organization](https://github.com/micro-decode) · [SkillHub](https://github.com/micro-decode/skillhub-platform) · [Growvia](https://github.com/micro-decode/growvia-analytics) · [AutoFlow](https://github.com/micro-decode/autonomous-execution)

</div>
