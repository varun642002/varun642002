<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:1e3a8a,100:22d3ee&height=180&section=header&text=Varun%20S.&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Business%20Analytics%20and%20Product%20Engineering&descAlignY=58&descSize=18" alt="Varun S. — Business Analytics and Product Engineering" width="100%" />

**Data analyst and full-stack developer.** I build analytics that people act on and the software systems behind them — SQL models, Power BI dashboards, production web and mobile apps — and I publish the developer tooling that falls out of the work: **12 open-source Claude Code plugins and hooks**, all MIT and zero-dependency.

[![Portfolio](https://img.shields.io/badge/Portfolio-1e3a8a?style=for-the-badge&logo=googlechrome&logoColor=white)](https://varun642002.github.io/varun-portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/varun64200/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/varun642002)

</div>

## About

I started in mechanical engineering, working on the brake system of a Formula Student car, before moving into data analytics and then into building complete software products. That background shapes how I work: measure first, understand what the data shows, then build the system that acts on it.

| | |
|---|---|
| **Focus** | Business intelligence, data analytics, full-stack product development |
| **Currently building** | IGNYT Coach (trainer management platform), the IGNYT iOS app, and open-source developer tooling |
| **Core stack** | Python, TypeScript, SQL, FastAPI, Next.js, PostgreSQL, Power BI |
| **Learning** | Azure data engineering |

---

## Open Source

Twelve tools for [Claude Code](https://claude.com/claude-code), built for my own
workflow and released because the problems are not mine alone. All MIT, all
zero-dependency Node, none of them phone home: no account, no server, nothing
leaves your machine.

```bash
claude plugin marketplace add varun642002/<name>
```

**Hooks — installed once, then they run on their own**

| | What it does |
|---|---|
| **[secretguard](https://github.com/varun642002/secretguard)** | Stops Claude Code reading secrets into its context. Blocks `.env` files, private keys and credential-shaped content *before* they reach the transcript — a secret in the context window is a secret in somebody's logs. |
| **[blastradius](https://github.com/varun642002/blastradius)** | Says what a change is about to reach. Warns before wide or sensitive edits, and never blocks. |
| **[testgate](https://github.com/varun642002/testgate)** | Never close a session on a red build. Runs the project's own type check and tests after any session that edited files. |

**Memory — so the next session starts knowing what the last one learned**

| | What it does |
|---|---|
| **[tinymem](https://github.com/varun642002/tinymem)** | Persistent project memory. Writes down what you taught it, hands it back at the next session start. Plain JSONL on your own disk. |
| **[recall](https://github.com/varun642002/recall)** | `grep` across every session you have ever had. Local full-text search over your transcripts. |

**Where the time and the tokens actually went**

| | What it does |
|---|---|
| **[tokenlens](https://github.com/varun642002/tokenlens)** | Token and cost analysis of your transcripts. Answers "why was that session expensive?" |
| **[standup](https://github.com/varun642002/standup)** | Builds your standup update from your git commits and your sessions. |

**Getting a project to run, and keeping it documented**

| | What it does |
|---|---|
| **[envdoctor](https://github.com/varun642002/envdoctor)** | Can this project actually run here? Checks runtime, package manager, dependencies, env var *names*, ports and git identity — and prints the command for whatever is missing. |
| **[claudemd-init](https://github.com/varun642002/claudemd-init)** | Writes a `CLAUDE.md` from what is actually in the repository. States only what it observed, with evidence for every claim. |
| **[prompt-kit](https://github.com/varun642002/prompt-kit)** | A shared, reviewed library of slash commands — scaffold a plugin repo your team installs, and lint the commands like source. |

**Agents, and the ecosystem around them**

| | What it does |
|---|---|
| **[lean-workflow](https://github.com/varun642002/lean-workflow)** | Ten token-lean agents and six workflow skills — plan, build, debug, test, review, secure, ship — each with a hard limit on what it reads and how much it reports. |
| **[claude-plugin-index](https://github.com/varun642002/claude-plugin-index)** | What the published plugins actually look like. A weekly, reproducible health report run with Claude Code's own validator. |

And one that is not a developer tool at all:

| | What it does |
|---|---|
| **[erp-starter-kit](https://github.com/varun642002/erp-starter-kit)** | A complete multi-branch ERP base — sales, stock, invoices, cash book, service, payroll, WhatsApp. React, TypeScript, Express, PostgreSQL, Firebase. Fork it and build your own. |

---

## Featured Projects

### 1. IGNYT Coach
![Status: Active](https://img.shields.io/badge/status-active-2ea043?style=flat-square)

A platform for personal trainers, gyms and nutrition coaches. Owners, trainers and assistants manage clients, build training programmes and meal plans, run check-ins, message clients and bill them. Assigned work syncs directly into the client-facing IGNYT app.

**Why it matters:** independent trainers and small gyms typically run their business across spreadsheets, group chats and separate payment tools. This consolidates programming, billing and communication into one system with role-based access.

<img src="https://skillicons.dev/icons?i=python,fastapi,postgres,nextjs,ts,docker" alt="Python, FastAPI, PostgreSQL, Next.js, TypeScript, Docker" />

[Repository](https://github.com/varun642002/ignyt-coach)

### 2. Ai-Data-Analytics-workspace
![Status: Experimental](https://img.shields.io/badge/status-experimental-2F81F7?style=flat-square)

An analytics workspace covering data profiling, cleaning, exploratory analysis, SQL querying, visualization and dashboards, with AI assisting the interpretation layer.

**Why it matters:** most analysis time goes into profiling and cleaning before any insight appears. This brings that setup work into a single workspace instead of a chain of notebooks and scripts.

<img src="https://skillicons.dev/icons?i=ts,python,postgres" alt="TypeScript, Python, SQL" />

[Repository](https://github.com/varun642002/Ai-Data-Analytics-workspace)

### 3. IGNYT — fitness and nutrition app
![Status: In development](https://img.shields.io/badge/status-in%20development-d29922?style=flat-square)

<a href="https://ignytfit.in"><img src="https://ignytfit.in/opengraph-image?f0472d49088eb765" width="100%" alt="IGNYT: workouts, nutrition, fasting, hydration and Health Connect in one app" /></a>

The client-facing side of IGNYT: a Next.js web app and a native iOS build (Swift, HealthKit integration, Codemagic CI) that receives programmes assigned by a coach in IGNYT Coach.

**Why it matters:** a trainer's plan only works if the client can follow it from their phone, with health data feeding back into the loop.

<img src="https://skillicons.dev/icons?i=nextjs,ts,swift" alt="Next.js, TypeScript, Swift" />

[Website](https://ignytfit.in) · [Web repository](https://github.com/varun642002/IGNYTfit.in) · [iOS repository](https://github.com/varun642002/Ignyt-ios)

### 4. Olist E-Commerce Sales Analysis
![Status: Completed](https://img.shields.io/badge/status-completed-6e7781?style=flat-square)

<img src="https://github.com/user-attachments/assets/b4fec4af-a522-416d-a67a-bbe307efcd38" width="100%" alt="Olist executive dashboard in Power BI showing revenue, orders, customers and top categories" />

Executive, Sales and Customer Insights dashboards built on the Olist Brazilian e-commerce dataset.

**Why it matters:** covers the full BI workflow — modeling raw transactional data, writing DAX measures, and presenting results for different audiences (executives, sales, customer operations).

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-217346?style=flat-square)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)

[Repository](https://github.com/varun642002/Olist-Ecommerce-Sales-Analysis-powerbi)

### 5. HR Workforce Analytics Dashboard
![Status: Completed](https://img.shields.io/badge/status-completed-6e7781?style=flat-square)

<img src="https://github.com/user-attachments/assets/c9671982-862f-4d71-abce-755658110752" width="100%" alt="HR workforce executive dashboard in Power BI showing headcount, attrition rate and satisfaction KPIs" />

A Power BI dashboard analyzing employee demographics, workforce distribution, attrition trends and satisfaction.

**Why it matters:** attrition is costly and often invisible until it becomes a problem; this surfaces the trend early enough for HR to act.

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-217346?style=flat-square)
![Power Query](https://img.shields.io/badge/Power_Query-217346?style=flat-square&logo=microsoftexcel&logoColor=white)

[Repository](https://github.com/varun642002/Hr-workforce-analytics-dashboard)

---

## Technical Skills

| | |
|---|---|
| **Languages** | Python, TypeScript, SQL, Swift |
| **Frontend** | React, Next.js, Tailwind CSS |
| **Backend** | FastAPI, Node.js |
| **Databases** | PostgreSQL, SQLite |
| **Data and BI** | Power BI, DAX, Power Query, Excel, Google Looker Studio |
| **Tooling** | Docker, GitHub Actions, Vercel, Codemagic |

<img src="https://skillicons.dev/icons?i=python,ts,swift,react,nextjs,tailwind,fastapi,nodejs,postgres,sqlite,docker,githubactions,vercel&perline=13" alt="Python, TypeScript, Swift, React, Next.js, Tailwind CSS, FastAPI, Node.js, PostgreSQL, SQLite, Docker, GitHub Actions, Vercel" />

---

## How I Work

- **Start from the user's problem.** IGNYT Coach exists because trainers run their business across several disconnected tools; the goal was to fix that, not to practice a framework.
- **Measure before optimizing.** Coming from BI, I look at the data before deciding on a fix.
- **Keep systems loosely coupled.** IGNYT Coach and the IGNYT app are separate repositories connected by a single HTTP contract, so each can change independently.
- **Ship the whole path.** A dashboard, backend, mobile client and the CI that deploys it — a project is finished when the last step works.
- **Automate the repetitive part.** tinymem and lean-workflow both came out of the same frustration: doing the same explaining, checking and reviewing by hand on every project.

---

## Timeline

```mermaid
flowchart LR
    A["Data and BI<br/>Power BI, SQL, DAX<br/>Jul 2026"] --> B["Full-stack product<br/>IGNYT Coach<br/>Jul - Aug 2026"]
    B --> C["Mobile and portfolio<br/>Swift, HealthKit<br/>Aug - Sep 2026"]
    C --> D["Developer tooling<br/>12 Claude Code tools<br/>Nov 2026"]
    D -.-> E["Next<br/>Scale IGNYT, deepen backend"]

    style A fill:#0f2027,stroke:#22d3ee,color:#ffffff
    style B fill:#1e3a8a,stroke:#22d3ee,color:#ffffff
    style C fill:#1d4ed8,stroke:#22d3ee,color:#ffffff
    style D fill:#2563eb,stroke:#22d3ee,color:#ffffff
    style E fill:#ffffff,stroke:#1e3a8a,stroke-dasharray:5 3,color:#1e3a8a
```

---

## GitHub Activity

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats.herokuapp.com/?user=varun642002&hide_border=true&background=0D1117&ring=22d3ee&fire=22d3ee&currStreakLabel=22d3ee&currStreakNum=ffffff&sideNums=c9d1d9&sideLabels=c9d1d9&dates=8b949e" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=varun642002&hide_border=true&ring=1e3a8a&fire=1e3a8a&currStreakLabel=1e3a8a" alt="GitHub contribution streak: total contributions, current streak and longest streak" width="90%" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/varun642002/varun642002/output/snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/varun642002/varun642002/output/snake.svg" />
  <img src="https://raw.githubusercontent.com/varun642002/varun642002/output/snake.svg" alt="Contribution graph animation generated from public GitHub activity" width="100%" />
</picture>

</div>

---

## Contact

I am open to data analyst, business intelligence and full-stack engineering opportunities.

- **LinkedIn:** [linkedin.com/in/varun64200](https://www.linkedin.com/in/varun64200/)
- **Portfolio:** [varun642002.github.io/varun-portfolio](https://varun642002.github.io/varun-portfolio/)
- **GitHub:** [github.com/varun642002](https://github.com/varun642002)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:22d3ee,50:1e3a8a,100:0f2027&height=80&section=footer" width="100%" alt="" />
