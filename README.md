# XinYi Ruan

**Data Science & Big Data Technology Undergraduate · AI Agent Developer · Full-Stack & Data Engineering**

Guangdong Peizheng College · School of Data and Computer Science · 2024 – 2028 · Guangzhou, China

**Blog**: [xin-yi33.github.io/By-My-Self](https://xin-yi33.github.io/By-My-Self/) · **GitHub**: [@xin-yi33](https://github.com/xin-yi33) · **Email**: ruanxinyi293@gmail.com

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Vue 3](https://img.shields.io/badge/Vue_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

## About Me

- Undergraduate in **Data Science and Big Data Technology** at Guangdong Peizheng College (2024 – 2028), GPA 3.55/4 — top 10% of the major.
- I build around **AI agents**: my flagship project [RxyCode](#rxycode) is a 100% local multi-agent workbench with ~150K lines of Python, three user surfaces and its own versioned RPC protocol.
- Hands-on across the whole pipeline: **data collection → analysis → modeling → product**, from JS-reverse web scrapers and Spark pipelines to PyTorch models and Flask/Vue full-stack apps.
- I work with AI agents daily (Claude Code, Codex, OpenCode, and my own), and design **Agent Skills / MCP** integrations rather than just using them.
- Student research project: **Individualized Agent — A Governed Self-Evolution Architecture for Personalized LLM Agents** (advisor: Li Jun), designing the storage, retrieval and safety architecture.

## Education

**Guangdong Peizheng College** — B.Eng. in Data Science and Big Data Technology, School of Data and Computer Science (2024 – 2028)

- **GPA**: 3.55 / 4 (top 10%)
- **Core coursework**: Python, Java, Data Structures & Algorithms, Mathematical Analysis, Linear Algebra, Probability & Statistics, Statistics, Linux, Database Principles & Applications, Web Front-end Development
- **Self-taught**: the big-data stack (Hadoop, Spark / PySpark, Hive / HiveQL, Scala), JavaWeb & backend (SpringBoot), BI analytics, the Baidu TianSuan big-data platform track, and AI-agent engineering (multi-agent orchestration, Skill / MCP design, prompt engineering, context management)

## Featured Open-Source Projects

### RxyCode

**[github.com/xin-yi33/RxyCode](https://github.com/xin-yi33/RxyCode)** — *A local multi-agent for real work, not just code.* (MIT · v1.3.0)

A 100% local, vendor-neutral AI agent workbench built from scratch: no cloud middleman, bring your own API key (encrypted with OS-native DPAPI / owner-only files), and support for 11 provider strategies — DeepSeek, Kimi, Qwen, Doubao, GLM, MiniMax, OpenAI, Anthropic and more.

- **Agent core** — a headless Python 3.10+ runtime (`Session` → `AgentV2`) driven by a LangGraph **plan → execute → validate → synthesize** pipeline with a fast path for simple turns; ~30 built-in tools (files, shell, git, web search/fetch, vision, downloads, LSP diagnostics, memory, scheduling).
- **Three surfaces, one protocol** — a Bun + React 19 terminal UI (OpenTUI), an Ink/React 18 fallback TUI, and an Electron 39 desktop workbench (Windows NSIS / portable, Linux AppImage), all speaking a Pydantic-defined **JSON-RPC 1.1.0 protocol** (141 request + 26 notification models) whose TypeScript types are code-generated from a frozen JSON schema — CI fails if the generated types drift. A FastAPI HTTP/SSE server exposes the same API headlessly.
- **Multi-agent system** — an Expert Team mode with 10 roles over 7 **deterministic** SOP stages (transitions are code, not LLM decisions), a mechanical verification gate of 8 hash-bound checks that runs before any LLM auditor, and budget fuses (tokens / wall-clock / delegations); isolated subagents get scoped tools, permissions and workspace leases.
- **Memory & RAG without heavy dependencies** — tiered short/long-term memory with a vector experience store; codebase RAG uses AST-aware chunking, a float32 NumPy cosine index and a PageRank repo map — no external vector database, no networkx.
- **Safety & reliability** — three-tier approval gate (auto-read, confirm-write, always-confirm-danger) with argument-aware risk classification, bash escape detection and a redacted audit log; a crash-safe **at-most-once side-effect journal**; durable checkpoints with rewind, thread fork and replayable JSONL traces.
- **Engineering discipline** — ~150K lines of Python (~80K product) and ~400K lines of TS/TSX; **12,876 backend tests** collected by pytest in 17 s; CI runs ruff, coverage gates (67% core), protocol drift checks, secret scanning, a real **Windows ConPTY end-to-end** suite, and a desktop build matrix; an evaluation harness benchmarks the agent against raw-LLM baselines — and team mode actually ships **off by default** because the maintainers measured that it costs ~3× tokens for no pass-rate gain.

### coding-agent-crew

**[github.com/xin-yi33/coding-agent-crew](https://github.com/xin-yi33/coding-agent-crew)** (MIT)

An Agent Skills pack that turns one AI session into a crew of seven hands-on engineer roles for building or improving Codex-shaped coding agents. Roles follow a two-track SOP (Create / Optimize) with hard ownership rules — e.g. surfaces may never grow a second agent loop, quality owns trajectory-eval gates, and implementers must test their own layer. Includes stack mapping to upstream skill packs and an installer that drops role routers into `.agents` / `.claude` / `.cursor` / `.grok`.

### novel-writer-skill

**[github.com/xin-yi33/-novel-writer-skill](https://github.com/xin-yi33/-novel-writer-skill)** (MIT)

A long-form Chinese web-novel writing engine shipped as an Agent Skill: outline → full chapters, with a memory architecture for serialization — character bibles, a summary-compression formula, 30-chapter arc consolidation and a rolling recent-chapter window — plus character consistency checks, writer's-block continuation, title generation and one-click draft publishing to the Fanqie Novel platform through browser MCP tools.

### gaokao

**[github.com/xin-yi33/gaokao](https://github.com/xin-yi33/gaokao)**

A full-stack college-application recommendation system ("reach / match / safety") in Flask + MySQL: 9 REST blueprints covering students, colleges, majors, rankings, industry trends, risk analysis and Excel/PDF export; a rank-difference probability model; and a multi-source collection suite built with Playwright, Selenium, Tesseract OCR and search-engine cross-validation.

## More Projects

- **RAG Knowledge-Base QA** — LangChain + DeepSeek + ChromaDB (1536-d DashScope embeddings), LCEL-orchestrated index/retrieve/generate pipeline with persistent multi-session memory.
- **YOLO Helmet-Detection System** — YOLOv1 implemented from scratch in PyTorch on a VGG16 backbone: custom weighted loss, full training and grid-decoding inference pipeline.
- **Real-Estate Market Analysis** — end-to-end analysis of 100K+ second-hand listings: cleaning, 10+ derived features, 7-dimension EDA and 10+ visualizations (pandas / seaborn).
- **Music-Site Data Collection** — reverse-engineered a request-signing algorithm (execjs + recovered MD5 logic) for batched scraping and automated audio downloads.
- **Retail Sales Analysis on Spark** — PySpark pipeline over JSON data with multi-metric aggregation written to both MySQL and Hive.

## Research

**Individualized Agent — A Governed Self-Evolution Architecture for Personalized LLM Agents** *(student research project, advisor: Li Jun)*

Designing a persistent personal-agent architecture where experience is distilled into governed knowledge objects (EKO) stored in a domain-partitioned B+ tree forest, retrieved by contextual routing, composed with dependency-aware planning, adjudicated by confidence scoring, and gated by safety policies before activation — with versioning, rollback and auditability at every step.

## GitHub Activity

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=xin-yi33&show_icons=true&hide_title=true&hide_border=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=xin-yi33&layout=compact&hide_title=true&hide_border=true)

## Contact

- **Blog**: [xin-yi33.github.io/By-My-Self](https://xin-yi33.github.io/By-My-Self/)
- **Email**: ruanxinyi293@gmail.com
- **GitHub**: [@xin-yi33](https://github.com/xin-yi33)
