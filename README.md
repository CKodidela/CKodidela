# Hi, I'm Chetan Reddy Kodidela 👋

Backend-focused software engineer graduating from **IIT Tirupati (May 2026)**.  
I work in production TypeScript codebases — cryptographic protocols, type-safe APIs, DB optimization, and system-boundary security.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/kchetanreddy)
[![LeetCode](https://img.shields.io/badge/LeetCode-%23006400.svg?logo=leetcode&logoColor=white)](https://leetcode.com/u/BROCODES2024/)
[![X](https://img.shields.io/badge/X-black.svg?logo=X&logoColor=white)](https://x.com/CKodidela)
[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:chetanreddyk394@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?logo=vercel&logoColor=white)](https://chetan-pp.vercel.app/)

---

## 🔧 What I Do

- **Open Source** — 12 merged PRs across [Nostream](https://github.com/Cameri/nostream) (Nostr relay) and [Galoy](https://github.com/GaloyMoney/galoy) (Bitcoin banking), reviewed and accepted by project maintainers
- **Cryptography** — Implemented NIP-44 v2 E2E crypto (ChaCha20, HKDF, MAC) from scratch in production
- **Performance** — Resolved N+1 queries with DataLoader batching; cut DB calls 12× with zero API contract changes
- **Type Safety** — Discriminated unions, Zod schemas, co-located auth checks — correctness at every layer

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
![WebSockets](https://img.shields.io/badge/WebSockets-black?style=flat&logo=websocket&logoColor=white)

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
- RBAC PostgreSQL schema (owner/contributor/mentor) with content gating — repo links only visible to approved members, enforced at the Server Action layer
- 4-stage GitHub Actions CI pipeline + Husky pre-commit hooks on staged files only

### [ZapRoom](https://zaproom.vercel.app) — Real-Time Chat App
`TypeScript` `Node.js` `WebSockets` `React` `shadcn/ui`

- Room-based chat with fan-out broadcast scoped to room members — O(room size) per message vs O(all connections) naive pattern
- Deliberate architectural decisions: connection isolation, efficient message routing

---

## 📊 Open Source Contributions

| Project | What I Did | Impact |
|---|---|---|
| [Nostream](https://github.com/Cameri/nostream) | NIP-44 v2 E2E crypto, relay-boundary access control, Zod migration, XSS fixes | Test coverage 21% → 88–93% (1,238 passing) |
| [Galoy](https://github.com/GaloyMoney/galoy) | Event-sourced Wallet module, N+1 query fix via DataLoader | DB calls cut from ~60 to ~5 per request (12×) |

---

## 🏆 Achievements

- 🥇 **LeetCode Knight** — Peak rating 1934, top 3.7%, 500+ problems
- ⚡ **Juspay Hiring Challenge** — Cleared 8/9 rounds from a pool of 200,000+ candidates
- 🏅 **Odoo Hackathon** — Ranked 41st out of 5,000+ teams
- 🎓 **Summer of Bitcoin** — Selected from 7,000+ applicants
- 📊 **Adobe Hackathon** — Top 4,000 out of 110,000+ teams
- ⭐ **CodeChef 3-Star** — Peak rating 1610

---

## 📈 GitHub Stats

![Chetan's GitHub Stats](https://github-readme-stats.vercel.app/api?username=chetan-pp&show_icons=true&theme=default&hide_border=true&count_private=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=chetan-pp&layout=compact&theme=default&hide_border=true)

---

*Targeting junior SDE roles in backend or systems engineering. If you're building something where performance, security, and correctness matter — let's talk.*
