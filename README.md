<div align="center">

# 🧠 PatternDSA
### Master DSA Patterns & System Design for Technical Interviews

[![Live Demo](https://img.shields.io/badge/Live%20Demo-patterndsa.vercel.app-10b981?style=for-the-badge&logo=vercel&logoColor=white)](https://patterndsa.vercel.app/)
[![Next.js 14](https://img.shields.io/badge/Next.js-14.2-black?style=for-the-badge&logo=next.js&logoColor=white)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.5-3178c6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-38bdf8?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Prisma ORM](https://img.shields.io/badge/Prisma-5.18-2d3748?style=for-the-badge&logo=prisma&logoColor=white)](https://www.prisma.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Neon-4169e1?style=for-the-badge&logo=postgresql&logoColor=white)](https://neon.tech/)

<p align="center">
  <strong>Stop memorizing 500+ random LeetCode solutions in isolation.</strong><br/>
  Master the underlying mental models, solve company-tagged problems, and ace technical interviews with automated spaced repetition.
</p>

[**Explore Live Platform »**](https://patterndsa.vercel.app/) · [Report Bug](https://github.com/aareeray/PatternDSA/issues) · [Request Feature](https://github.com/aareeray/PatternDSA/issues)

</div>

---

## 🚀 The Philosophy: Why PatternDSA?

Most software engineers fail coding interviews not because they didn't grind enough problems, but because they **solve problems in isolation without recognizing the recurring mental models**.

| Traditional LeetCode Grinding ❌ | The PatternDSA Approach ✅ |
| :--- | :--- |
| Memorizing 500+ individual problem tricks | Mastering **25+ core algorithmic patterns** |
| Blanking out when an interviewer tweaks constraints | Recognizing pattern signals and execution recipes |
| Forgetting solutions 2 weeks after solving | **Automated Spaced Repetition** (Day 1 $\rightarrow$ 3 $\rightarrow$ 7 $\rightarrow$ 14 $\rightarrow$ 30) |
| Single language solutions | **4-Language Production Blueprints** (C++, Java, Python, JS) |
| Coding-only preparation | Full-stack prep: **DSA + SQL + Core CS + System Design** |

---

## ✨ Key Platform Features

### 1. 🎯 Pattern-Based Algorithmic Curriculum
- Organized hierarchically into **Topics ➔ Patterns ➔ Canonical Benchmark Problems**.
- Comprehensive pattern guides featuring:
  - **Identification Signals**: Keywords and constraint cues that reveal the optimal pattern.
  - **Execution Recipe**: Step-by-step algorithmic blueprint before writing code.
  - **When NOT to Use**: Traps and anti-patterns that lead to suboptimal complexity.
  - **Multi-Language Blueprints**: Production-ready code templates in **C++**, **Java**, **Python**, and **JavaScript**.

### 2. 🏢 620+ Company-Tagged Problems Sheet
- Curated pattern-wise question sheet with company tags and logos:
  - **FAANG / Big Tech**: Google, Microsoft, Amazon, Meta, Apple, Netflix
  - **Unicorns & High-Growth**: Uber, Adobe, Goldman Sachs, Flipkart, Salesforce, Atlassian, Bloomberg
- Filter by **Difficulty** (*Easy, Medium, Hard*), **Status** (*Solved, Unsolved*), and **Search Keywords**.
- One-click deep-linking to LeetCode and GeeksforGeeks platforms.

### 3. 📚 Domain Interview Knowledge Base (1:1 Interactive Notes)
Master core Computer Science fundamentals with structured modules and interactive practice questions:
- **SQL (85+ curated questions)**: SELECT, WHERE, GROUP BY, Window Functions, Self Joins, CTEs, Index optimization.
- **System Design Primer**:
  - The 4-Step Technical Interview Framework & Latency Numbers.
  - Distributed consistency (CAP, PACELC, Weak vs Eventual vs Strong).
  - High availability, Load balancing (L4 vs L7), Consistent Hashing, Push/Pull CDNs.
  - Caching strategies (Cache-Aside, Write-Through, Write-Behind) & Cache Stampede mitigation.
  - Real-world case studies: **Pastebin / TinyURL** and **Twitter Timeline Fan-out**.
- **DBMS**: ACID properties, Transaction isolation levels, Concurrency control, B+ Trees vs Hash indexing.
- **Operating Systems**: Processes vs Threads, CPU scheduling, Virtual memory, Paging, Deadlocks.
- **Computer Networks**: OSI & TCP/IP stack, DNS, TCP 3-way handshake, TLS/HTTPS, WebSockets.

### 4. ⏱️ Automated Spaced Repetition (SRS Engine)
- Combat the **Ebbinghaus Forgetting Curve**.
- When you mark a problem solved, PatternDSA schedules personalized review sessions:
  $$\text{Solved} \longrightarrow \text{Day 1} \longrightarrow \text{Day 3} \longrightarrow \text{Day 7} \longrightarrow \text{Day 14} \longrightarrow \text{Day 30}$$
- Daily review queues ensure algorithms transition from short-term memory to permanent intuition.

### 5. 📰 Engineering Articles & Knowledge Sharing
- Read and publish deep-dive technical articles across categories:
  - *System Design*, *Data Structures & Algorithms*, *Core CS*, *Database Internals*, *DevOps*, *GenAI*.
- Interactive markdown reader, bookmarking, and discussion comments.

---

## 🛠️ Technology Stack

```
PatternDSA
├── Frontend:     Next.js 14 (App Router) + React 18 + TypeScript 5
├── Styling:      Tailwind CSS 3.4 + shadcn/ui + Lucide Icons
├── Backend:      Next.js Route Handlers (Edge & Node.js Serverless)
├── Validation:   Zod 3.23 (Strict runtime schema validation)
├── Database:     PostgreSQL (Production via Neon) / SQLite (Local Dev)
├── ORM:          Prisma ORM 5.18 (Type-safe migrations & queries)
├── Auth:         JWT (HttpOnly access & refresh tokens) + bcryptjs
└── Hosting:      Vercel Serverless Platform
```

---

## 🏛️ System Architecture

```mermaid
graph TD
    subgraph Clients ["👥 User Interfaces"]
        Browser["💻 Web Browser (Desktop / Mobile)"]
    end

    subgraph Edge ["⚡ Vercel Edge & Serverless"]
        Router["Next.js 14 App Router"]
        AuthMiddleware["🔒 Auth & Cookie Middleware"]
        API["REST API Handlers (/api/v1/*)"]
    end

    subgraph Modules ["📦 Application Modules"]
        PatternsMod["🧠 Pattern Engine"]
        ProblemsMod["🧩 Problem Catalog (620+ Problems)"]
        DomainMod["📚 Domain Knowledge (SQL, OS, System Design)"]
        RevisionMod["⏱️ Spaced Repetition Queue"]
        ArticlesMod["📰 Engineering Articles"]
    end

    subgraph Storage ["🗄️ Persistence Tier"]
        Prisma["💎 Prisma ORM Client"]
        Database[("🐘 PostgreSQL / Neon Database")]
    end

    Browser -->|HTTPS| Router
    Router --> AuthMiddleware
    AuthMiddleware --> API
    API --> PatternsMod
    API --> ProblemsMod
    API --> DomainMod
    API --> RevisionMod
    API --> ArticlesMod
    PatternsMod --> Prisma
    ProblemsMod --> Prisma
    DomainMod --> Prisma
    RevisionMod --> Prisma
    ArticlesMod --> Prisma
    Prisma --> Database
```

---

## 🏁 Getting Started (Local Development)

### 1. Prerequisites
- **Node.js**: `v18.17+` or `v20+`
- **npm**: `v9+` or `pnpm` / `yarn`
- **Git**

### 2. Clone Repository
```bash
git clone https://github.com/aareeray/PatternDSA.git
cd PatternDSA
```

### 3. Install Dependencies
```bash
npm install
```
*(This automatically runs `postinstall: prisma generate` to build the type-safe database client)*.

### 4. Configure Environment Variables
Create a `.env` file in the root directory:
```bash
cp .env.example .env
```
Populate your secrets:
```env
# Server & Client
NODE_ENV=development
CLIENT_URL="http://localhost:3000"

# Database (Neon PostgreSQL or local PostgreSQL)
DATABASE_URL="postgresql://username:password@ep-xxxx.neon.tech/neondb?sslmode=require"

# JWT Authentication
JWT_ACCESS_SECRET="your_custom_jwt_access_secret_32_chars_min"
JWT_REFRESH_SECRET="your_custom_jwt_refresh_secret_32_chars_min"
ACCESS_TOKEN_EXPIRES="15m"
REFRESH_TOKEN_EXPIRES="7d"
```

### 5. Setup Database & Seed Initial Data
Push the schema to your database and auto-seed all problems, patterns, and articles:
```bash
npx prisma db push
node prisma/seed-production.mjs
```

### 6. Start the Development Server
```bash
npm run dev
```
Open **[http://localhost:3000](http://localhost:3000)** in your browser to start learning!

---

## 🚢 Deploying to Vercel (Production)

PatternDSA is fully optimized for **zero-friction Vercel deployment**:

1. Fork or push this repository to your GitHub account.
2. Go to **[vercel.com/new](https://vercel.com/new)** and import **`PatternDSA`**.
3. Under **Environment Variables**, provide:
   - `DATABASE_URL`: Your cloud PostgreSQL connection string (free from [Neon.tech](https://neon.tech) or [Supabase](https://supabase.com)).
   - `JWT_ACCESS_SECRET`: A secure random 32-character string.
   - `JWT_REFRESH_SECRET`: A secure random 32-character string.
   - `NODE_ENV`: `production`.
4. Click **Deploy**.
   - Vercel automatically runs `prisma db push` to generate tables.
   - Vercel automatically runs `seed-production.mjs` to populate all 620+ problems and patterns.
   - The platform goes live with full registration, login, and progress tracking!

---

## 📈 Platform Roadmap

- [x] 130+ Algorithmic Patterns with 4-Language Blueprints
- [x] 620+ Company-Wise Problem Sheet with Real Company Logos
- [x] Full Domain Study Section: SQL, DBMS, OS, Computer Networks
- [x] Complete System Design Primer Notes & Architecture Blueprints
- [x] Ebbinghaus Spaced Repetition Tracker
- [x] Dark/Light Mode Theme Engine
- [ ] Interactive Monaco Code Editor with Live Sandboxed Execution
- [ ] AI-Powered Code Explainer & Big-O Complexity Analyzer
- [ ] Peer-to-Peer Mock Technical Interview Rooms

---

## 👨‍💻 Creator & Credits

Engineered and maintained with ❤️ by **Ayaan**:

- **Instagram**: [@ayaan.ji_](https://www.instagram.com/ayaan.ji_)
- **GitHub**: [@aareeray](https://github.com/aareeray)
- **Live Deployment**: [https://patterndsa.vercel.app/](https://patterndsa.vercel.app/)

Special thanks to the open-source community, LeetCode, and the System Design Primer for algorithmic references.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE). Feel free to learn from, fork, and build upon it!

<div align="center">
  <sub>⭐ If PatternDSA helps you in your technical interview journey, consider giving this repo a star!</sub>
</div>
