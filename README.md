# Hi, I'm Chetan Reddy Kodidela 👋

Backend engineer graduating from **IIT Tirupati (May 2026)**.
I build in production TypeScript codebases: cryptographic protocols, type-safe APIs, query optimization, and security at the system boundary.
Currently expanding into AI engineering, exploring LLM tooling and agent infrastructure.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/kchetanreddy)
[![LeetCode](https://img.shields.io/badge/LeetCode-%23006400.svg?logo=leetcode&logoColor=white)](https://leetcode.com/u/BROCODES2024/)
[![X](https://img.shields.io/badge/X-black.svg?logo=X&logoColor=white)](https://x.com/CKodidela)
[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:chetanreddyk394@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?logo=vercel&logoColor=white)](https://chetan-pp.vercel.app/)

---

## 🔧 What I Work On

- **Production backend systems** in TypeScript/Node.js: relay infrastructure, event-sourced architectures, WebSocket servers
- **Cryptographic protocol implementation**: E2E encryption schemes, key derivation, MAC verification from spec
- **Database performance**: query batching, schema design, ORM optimization across PostgreSQL and MongoDB
- **Type safety and correctness**: discriminated unions, Zod validation, co-located auth checks that can't be bypassed
- **AI engineering** (learning): LLM APIs, agent workflows, prompt engineering, tool use

---

## 🛠️ Tech Stack

**Languages**
![TypeScript](https://img.shields.io/badge/TypeScript-%23007ACC.svg?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=flat&logo=c%2B%2B&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-%23000000.svg?style=flat&logo=rust&logoColor=white)

**Backend**
![Node.js](https://img.shields.io/badge/Node.js-6DA55F?style=flat&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-%23404d59.svg?style=flat&logo=express&logoColor=%2361DAFB)
![WebSockets](https://img.shields.io/badge/WebSockets-black?style=flat)

**Frontend**
![Next.js](https://img.shields.io/badge/Next.js-black?style=flat&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-%2338B2AC.svg?style=flat&logo=tailwind-css&logoColor=white)

**Databases**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-%23316192.svg?style=flat&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=flat&logo=mongodb&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white)

**DevOps & Tools**
![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-%232671E5.svg?style=flat&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-%23000000.svg?style=flat&logo=vercel&logoColor=white)

---

## 🚀 Featured Projects

### [Brikrow](https://brikrow.vercel.app) — Collaborative Dev Portfolio Platform
`Next.js` `TypeScript` `PostgreSQL` `Prisma` `Supabase Auth` `Tailwind CSS v4`

- Developers post projects, recruit contributors (capped at 3/project), and apply as mentors
- Role-enforced PostgreSQL schema (owner/contributor/mentor RBAC) with unique membership constraints; repo links gated to approved members only, enforced at the Server Action layer to avoid round-trip latency
- 4-stage GitHub Actions CI pipeline (install, lint/format, type-check, build) with Husky pre-commit hooks scoped to staged files only

### [ZapRoom](https://zaproom.vercel.app) — Real-Time Chat App
`TypeScript` `Node.js` `WebSockets` `React` `shadcn/ui`

- Fan-out broadcast iterates only over room members, keeping per-message cost O(room size) vs the O(all connections) naive pattern
- Deliberate design: connection isolation and efficient message routing built in from the start, not bolted on

---

## 🔐 Open Source Contributions

### [Nostream](https://github.com/Cameri/nostream) — Nostr Protocol Relay
> High-performance relay infrastructure for the Nostr decentralized social protocol

- **NIP-44 v2 encryption** — Implemented ChaCha20-Poly1305 + HKDF key derivation + MAC verification from scratch, replacing the legacy NIP-04 path that had metadata leaks and weak key derivation
- **Relay-boundary access control (NIP-17)** — Blocked inner event kinds 13/14/15 at the relay layer regardless of client behavior, preventing unencrypted DMs from ever reaching the DB
- **Type-safe CLI refactor** — Rewrote `runCommandWithOutput` as a `CommandResult` discriminated union, eliminating per-call-site try/catch and making spawn failures type-safe across all CLI commands
- **Marmot Protocol support (MIPs 00-03)** — Added E2EE group messaging with 5 event kind handlers and a `GroupEventStrategy` that validates required group-ID tags; relay operates transport-only with no MLS logic
- **Performance + validation** — Optimized NIP-25 tag validation from multiple `.find()` calls to a single O(n) pass; migrated all 8 schemas from Joi to Zod, removing the Joi dependency entirely
- **Reliability** — Fixed a 301 permanent-redirect bug on the relay home page, added XSS prevention via HTML escaping, and in-memory template caching. Raised unit test coverage from ~21% to 88-93% (1,238 passing tests)

### [Galoy](https://github.com/GaloyMoney/galoy) — Bitcoin Banking Infrastructure
> Open-source backend powering Bitcoin banking applications

- **Event-sourced Wallet module** — Replaced mutable DB state with an append-only event log, enabling full audit history and zero-downtime state replay without API contract changes
- **N+1 query elimination** — Introduced DataLoader batching on the transaction-history endpoint, cutting DB calls from ~60 to ~5 per request (12x reduction) with no changes to the API surface

---

## 🤖 Currently Learning: AI Engineering

Exploring the infrastructure side of AI systems:

- LLM API integration (tool use, structured outputs, multi-turn context management)
- Agent architectures and workflow orchestration
- Retrieval-augmented generation (RAG) and vector search
- Prompt engineering and evaluation

*Goal: bring the same correctness-first mindset from backend systems into AI application development.*

---

## 🏆 Achievements

- 🥇 **LeetCode Knight** — Peak rating 1934, top 3.7%, 500+ problems solved
- ⚡ **Juspay Hiring Challenge** — Cleared 8 of 9 rounds from a national pool of 200,000+ candidates
- 🏅 **Odoo Hackathon** — Ranked 41st out of 5,000+ teams
- 🎓 **Summer of Bitcoin** — Selected from 7,000+ applicants (3-stage competitive process)
- 📊 **Adobe Hackathon** — Top 4,000 out of 110,000+ teams
- ⭐ **CodeChef 3-Star** — Peak rating 1610

---

## 📈 GitHub Stats

![Chetan's GitHub Stats](https://github-readme-stats.vercel.app/api?username=CKodidela&show_icons=true&theme=default&hide_border=true&count_private=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=CKodidela&layout=compact&theme=default&hide_border=true)

---

*Targeting junior SDE roles in backend or systems engineering. Open to AI engineering opportunities too. If you're building something where performance, security, and correctness matter, let's talk.*
