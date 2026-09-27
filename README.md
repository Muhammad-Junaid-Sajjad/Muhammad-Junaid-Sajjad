<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,25:0A192F,55:16324F,80:1B4B8C,100:2E8BFF&height=230&section=header&text=Muhammad%20Junaid%20Sajjad&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Forward%20Deployed%20Engineer%20%7C%20Agentic%20AI%20Engineer%20%7C%20Founder%2C%20AI-Native%20Cybersecurity%20Engineering&descAlignY=58&descSize=16" width="100%"/>

<a href="https://github.com/Muhammad-Junaid-Sajjad">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=21&pause=1500&color=D4AF37&center=true&vCenter=true&width=1000&repeat=false&separator=;&lines=Founding+Engineer+%40+Mellox+AI+(formerly+RavalAI);Founder+%40+AI-Native+Cybersecurity+Engineering;Building+the+System+of+Record+for+the+Agentic+Era;Solo-built+OpenClaw%3A+WhatsApp+%E2%86%92+Claude+%E2%86%92+MCP+routing;PIAIC+Agent+Factory+%E2%80%94+Forward+Deployed+Engineer+track;Security-first+%C2%B7+Spec-driven+%C2%B7+Always+shipping" alt="Typing SVG" />
</a>

</div>

<br/>

## 🛡️ Founder — AI-Native Cybersecurity Engineering

<div align="center">
<a href="https://www.linkedin.com/company/ai-native-cybersecurity-engineering/">
<img src="https://sc02.alicdn.com/kf/Acb73d6ac3c7f44b59ca10d58831d7df7V.png" width="100%" alt="AI-Native Cybersecurity Engineering — The System of Record for the Agentic Era"/>
</a>
</div>

> **Intelligence. Automation. Protection.**
> I'm the founder of **AI-Native Cybersecurity Engineering** — building the **System of Record (SoR)** for cybersecurity in the agentic era, where autonomous AI agents don't just detect threats. They reason about them, act on them, and leave an auditable trail.

- 🧠 **Thesis** — security tooling built *for* AI agents and *by* AI agents. AI-native from the ground up, not AI bolted onto legacy stacks.
- 📒 **SoR-first** — every autonomous security action should be recorded, auditable, and replayable. No agent action should be a black box.
- 🚧 **Status: early / building in public** — the SoR platform is currently a local build (not yet publicly deployed); this README is a founder's build log, not a shipped product page.
- 🔗 [AI-Native Cybersecurity Engineering — LinkedIn](https://www.linkedin.com/company/ai-native-cybersecurity-engineering/)

<br/>

## 👋 About Me

> Founder by conviction, engineer by habit. I take systems from ambiguous requirements to production — architecture, implementation, security, testing, deployment, and stakeholder communication, end to end.

I'm a CS undergrad (7th semester) at Lahore Garrison University, Pakistan, and the founder of **AI-Native Cybersecurity Engineering**. At **Mellox AI** (formerly RavalAI), I went from intern to **Founding Engineer**, with sole technical ownership of the Social Distribution Engine — a production FastAPI/PostgreSQL/Redis/Celery platform integrated with multiple social networks.

I'm training as a **Forward Deployed Engineer (FDE)** under **Panaversity's Agent Factory** — the spec-driven, human-supervised curriculum for building **Digital FTEs**: AI workers built to replace or augment a human full-time role.

My build process is spec-first. I call it **SDD-RI** — Specification-Driven Development with Recursive Intelligence: write the spec, build in small verifiable loops, audit and refine against real requirements, repeat. I authored a 5,710-word IEEE-style research paper on it, backed by a mixed-methods study across 12 workflow executions and 108 tasks.

Terminal-first on Ubuntu. **Claude Code** is my primary build agent — spec-driven development end-to-end, not autocomplete-assisted coding.

- 🏗️ **Founding Engineer @ Mellox AI** — owned a production system across 8 build phases, 166 automated tests (153 unit, 13 E2E), queue-first architecture with FastAPI + PostgreSQL + Redis + Celery + Docker Compose
- 🛡️ Founding **AI-Native Cybersecurity Engineering** — the SoR for autonomous, agent-driven security
- 🤖 Design and ship agentic systems that reason, plan, and route tools across APIs — **OpenClaw** is the proof
- 📐 Apply **SDD-RI** — structured specs before implementation, empirically validated against real task-completion data
- 🔐 Production security work — Fernet-encrypted OAuth tokens at rest, HMAC-SHA256 webhook signing, idempotency keys, typed failure classification, pre-launch code auditing
- 🧩 Studying MCP-based tool-routing and Claude's Skills/Subagents architecture, and applying it to my own agent designs
- 🎓 Teaching & mentorship — part-time instructor at a private academy (2024–2026) and peer mentor guiding 15+ CS students at LGU

<br/>

## 🤖 Agentic & Multi-Agent Architecture — What I'm Building Toward

I think about agent systems in layers, not as one monolithic "agent":

```
Harness            ← the runtime an agent lives in (Claude Code, or one you build)
 └── Main Agent     ← the primary worker inside the harness
      ├── Skills        ← in-context, task-specific instructions loaded on demand
      ├── Subagents      ← isolated workers with their own context window
      └── Agent Teams    ← multiple agents coordinating on a shared goal
Hooks & Plugins     ← cut across every layer — deterministic control points
                       and extended tool access, regardless of which layer fires
```

Why this matters, in practice:
- **Context isolation** — a single agent's context window degrades as it accumulates irrelevant history. Subagents give each subtask a clean, dedicated context, which is what makes parallel work (research, multi-file refactors, multi-source synthesis) viable instead of one long degrading thread.
- **Skills vs. subagents** — skills are cheap: markdown loaded into the *same* context only when relevant, replacing repetitive prompting. Subagents cost more (a new context, a round-trip) but buy isolation. Knowing which one a task actually needs is most of the architecture decision.
- **Where the speedup comes from** — Anthropic's own multi-agent research system (Opus as lead, Sonnet subagents) beat a single-agent Opus setup by ~90% on internal evals, largely because independent context windows let subagents reason in parallel instead of serially.
- **Hooks** — deterministic, code-level control points at an agent's lifecycle events (before a tool call, after a response) that can't be reasoned around the way a prompt instruction can. This is what turns "the model usually behaves" into "the system guarantees a boundary" — which is exactly the property security-facing agent tooling needs.

I'm actively studying this stack (Claude's Skills / Subagents / Agent Teams model, and the harness/hooks/plugins layer around it) and folding it into how I design **OpenClaw** and the future AI-Native Cybersecurity Engineering agent tooling — this section reflects architecture I'm building toward, not a shipped multi-agent product.

<br/>

## 📒 SoR, KSoR & DSoR — the Governance Layer Behind Agentic Systems

A **System of Record (SoR)** is the thing an organization treats as ground truth — the record everyone, including an AI agent, defers to. For autonomous agents specifically, two complementary ideas (from Panaversity's open-source `ksor` and `dsor` projects, which I've studied closely) frame what a *governed* SoR needs to do:

- **KSoR (Knowledge System of Record)** — an authoritative, governed knowledge layer for humans and agents to answer *from*. The key distinction: a knowledge base merely stores information; a KSoR establishes **authority** — provenance, citations, versioning, and the ability to abstain when it doesn't know, treated as architecture, not optional extras.
- **DSoR (Data System of Record)** — the governed layer between an agent and an organization's real systems (ERP, accounting, databases). It never takes an agent's word for anything: it checks permissions itself, requires human sign-off on large actions, prevents duplicate actions, and keeps an audit trail — because an agent can be confidently wrong or manipulated by text it reads, and will retry things a human wouldn't.

This is the conceptual foundation I'm building **AI-Native Cybersecurity Engineering**'s own SoR thinking on: security actions taken by autonomous agents need the same governed, audited, non-repudiable trail — applied to threat detection and response instead of general business operations.

<br/>

<details>
<summary>🚧 What I'm currently working on</summary>
<br/>

- Laying the foundation of **AI-Native Cybersecurity Engineering** — vision, architecture, and the SoR core, including an early local build of the platform site (not yet public)
- **Founding Engineer at Mellox AI** (formerly RavalAI) — sole technical ownership of the Social Distribution Engine, from architecture through production deployment
- Independent client-facing engineering work across small business and university contexts — requirements discovery through deployment
- Actively training as a **Forward Deployed Engineer** through **Panaversity's Agent Factory**
- Studying Claude's Skills / Subagents / Agent Teams architecture and Panaversity's KSoR/DSoR governance model, and applying both to my own agent designs
- Sketching a long-term vision for an **Autonomous Agentic Operating System (AAOS)** — a self-evolving, agent-scheduled OS built on Linux

</details>

<details>
<summary>⚡ Fun facts</summary>
<br/>

- Wrote a self-published paper on spec-driven development before finishing my degree
- Ubuntu + terminal only, no IDE training wheels
- Currently vision-boarding an entire agent-scheduled operating system, because the idea won't leave me alone

</details>

<br/>

## 🧰 Tech Stack

<div align="center">

`LANGUAGES`

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

`FRAMEWORKS`

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Docusaurus](https://img.shields.io/badge/Docusaurus-16324F?style=for-the-badge&logo=docusaurus&logoColor=white)

`AI & AGENTIC STACK`

![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![Claude Agent SDK](https://img.shields.io/badge/Claude%20Agent%20SDK-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-2E8BFF?style=for-the-badge)
![Skills & Subagents](https://img.shields.io/badge/Skills%20%26%20Subagents-16324F?style=for-the-badge)
![Hooks](https://img.shields.io/badge/Hooks-16324F?style=for-the-badge)
![OpenClaw](https://img.shields.io/badge/OpenClaw-0A192F?style=for-the-badge)

`SECURITY`

![Secure Auth](https://img.shields.io/badge/Secure%20Auth-0A192F?style=for-the-badge&logo=springsecurity&logoColor=2E8BFF)
![Secrets Management](https://img.shields.io/badge/Secrets%20Management-16324F?style=for-the-badge&logo=vault&logoColor=white)
![Code Audit](https://img.shields.io/badge/Code%20Audit-2E8BFF?style=for-the-badge&logo=owasp&logoColor=white)

`ML & DATA`

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-16324F?style=for-the-badge)

`DATABASES, INFRA & QA`

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)

</div>

<br/>

## 🎓 Forward Deployed Engineer Training — Panaversity Agent Factory

- **Program:** Panaversity Agent Factory — Digital FTE manufacturing, deployable specification-first AI systems
- **Track:** Forward Deployed Engineer (FDE) — vendor-neutral, spec-driven, human-supervised agent engineering
- **Status:** In progress — methods applied directly to production work through **OpenClaw**
- **Also studying:** Claude's Skills/Subagents/Agent Teams model and governed-record architecture (KSoR/DSoR), folded into OpenClaw's design and the early architecture of AI-Native Cybersecurity Engineering

<br/>

## 📊 GitHub Stats & Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Muhammad-Junaid-Sajjad&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=D4AF37&icon_color=2E8BFF&text_color=C9D1D9&include_all_commits=true&count_private=true" width="49%" alt="GitHub stats"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Muhammad-Junaid-Sajjad&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=D4AF37&text_color=C9D1D9&langs_count=8" width="41%" alt="Top languages"/>

<br/><br/>

<img src="https://streak-stats.demolab.com/?user=Muhammad-Junaid-Sajjad&theme=tokyonight&hide_border=true&background=0D1117&stroke=D4AF37&ring=D4AF37&fire=2E8BFF&currStreakLabel=D4AF37&sideLabels=C9D1D9&dates=8B949E" width="70%" alt="GitHub streak"/>

<br/><br/>

<img src="https://github-profile-trophy.vercel.app/?username=Muhammad-Junaid-Sajjad&theme=discord&no-frame=true&no-bg=true&row=1&column=7&margin-w=8" width="100%" alt="GitHub trophies"/>

</div>

<br/>

## 🚀 Featured Projects

| Project | What it does | Stack |
|---|---|---|
| 🏗️ **Social Distribution Engine** — Mellox AI | Founding Engineer, sole technical ownership. 8 build phases, 166 automated tests (153 unit, 13 E2E). Queue-first architecture with row-level locking (`SELECT FOR UPDATE SKIP LOCKED`) to prevent double-posting; Fernet-encrypted OAuth tokens, HMAC-SHA256 webhook signing, idempotency keys | `FastAPI` `PostgreSQL` `Redis` `Celery` `Docker Compose` |
| 🛡️ **[AI-Native Cybersecurity Engineering (SoR)](https://www.linkedin.com/company/ai-native-cybersecurity-engineering/)** | Founder — building the System of Record for autonomous, agent-driven cybersecurity. Early stage, building in public. | `Agentic AI` `Security` `SoR` |
| 🤖 **[OpenClaw — WhatsApp Agentic Gateway](https://github.com/Muhammad-Junaid-Sajjad)** | Claude as the reasoning layer for a WhatsApp gateway that autonomously selects and invokes tools. MCP-based tool routing, SKILL.md agent-definition patterns. Deployed as a persistent `systemd` service on Ubuntu | `Python` `Claude` `MCP` |
| 🦾 **[Physical AI & Humanoid Robotics Textbook](https://muhammad-junaid-sajjad.github.io/Hackathon1/)** | Solo-built, live interactive platform. 4 modules, 12 chapters, 87+ sections covering ROS 2, NVIDIA Isaac Sim, Gazebo, and VLA robot control. FastAPI + LangChain + Qdrant RAG chatbot and personalization engine ([repo](https://github.com/Muhammad-Junaid-Sajjad/Hackathon1)) | `Docusaurus` `React` `TypeScript` `LangChain` `Qdrant` |
| 🗳️ **[LGU MUN 2026 — Delegate Registration Platform](https://github.com/Muhammad-Junaid-Sajjad/LguMun)** | Concurrency-safe registration (`SELECT FOR UPDATE`), load-tested for 450 concurrent delegates, pre-launch audit resolving 9 defects, 98% Playwright E2E pass rate (41/42) | `FastAPI` `PostgreSQL` |
| 📄 **[SDD-RI Research](https://github.com/Muhammad-Junaid-Sajjad/AI-Spec-Driven-Development)** | 5,710-word IEEE-style paper introducing Specification-Driven Development with Recursive Intelligence. Mixed-methods study: 12 workflow executions, 108 tasks, 91.7% task-completion rate, 4.2/5.0 adherence score | `Research` |
| 🩺 **[Chronic Kidney Disease Prediction (ML)](https://github.com/Muhammad-Junaid-Sajjad/CCP_ML_Theory)** | Academic group project. Independently led preprocessing, feature selection, and model comparison across Random Forest, XGBoost, and a Voting Classifier | `scikit-learn` `XGBoost` |
| ⚙️ **[Hybrid CPU](https://github.com/Muhammad-Junaid-Sajjad/Ai-based--Hybrid-architectural-project-) & [RISC Simulator](https://github.com/Muhammad-Junaid-Sajjad/Mips_Project_01)** | Two interactive CPU simulators in vanilla JS, including a custom instruction-fusion design | `JavaScript` |

<br/>

## 📫 Let's Connect

<div align="center">

[LinkedIn](https://www.linkedin.com/in/muhammad-junaid-95742925a/) &nbsp;·&nbsp; [Company Page](https://www.linkedin.com/company/ai-native-cybersecurity-engineering/) &nbsp;·&nbsp; [GitHub](https://github.com/Muhammad-Junaid-Sajjad) &nbsp;·&nbsp; [Email](mailto:junaidsajjad2298@gmail.com)

**Founding Engineer @ Mellox AI · Founder @ AI-Native Cybersecurity Engineering · Open to FDE opportunities & collaborations**

<sub>💬 Let's build the security layer of the agentic era — together.</sub>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2E8BFF,50:16324F,100:000000&height=100&section=footer" width="100%"/>
