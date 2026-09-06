<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&pause=1000&color=F75C7E,6E4B7C,00B2B1&center=true&vCenter=true&width=700&lines=AI+Engineer+%26+Backend+Developer;Building+RAG+systems+that+measure%2C+not+just+answer;Local-first+AI+agents%2C+private+by+design;From+FastAPI+pipelines+to+statistically+significant+evals" alt="Typing SVG" />
</p>

<h1 align="center">Hi, I'm Ertürk Eryavuz 👋</h1>

<p align="center">
  <a href="https://linkedin.com/in/erturkeryavuz"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="mailto:erturkeryavuz@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

---

### 🧭 About Me

I build backend systems and AI-powered applications — FastAPI services, LLM integrations, and the retrieval/data pipelines underneath them. Most recently at **Eczacıbaşı–Esan**, where I built Python reporting pipelines and AI chatbot solutions on Microsoft Copilot Studio, and shipped an internal analytics assistant powered by DeepSeek.

- 🔭 **Currently building:** RAG Platform & NEXUS — my two active projects (see below)
- 🌱 **Deepening skills in:** LLM systems, retrieval architectures, agentic tool-calling, and SwiftUI
- 🤝 **Open to:** backend, AI engineering, and automation-driven projects
- 🎓 Computer Engineering, Maltepe University — graduation project: AI-driven fantasy basketball app with LLM integration

---

### 🧪 Highlighted Projects (active)

#### 🔍 RAG Platform *(private repo — happy to walk through the code or share access on request)*

A production-minded Retrieval-Augmented Generation system, built around the question most RAG demos skip: **how do you know it's actually right?** Not just "it answers" — it *measures* retrieval quality, grounding, cost, and latency, and reports honest results even when they're negative.

![Hybrid Retrieval](https://img.shields.io/badge/Hybrid%20Retrieval-Dense%20%2B%20BM25%20%2B%20RRF-6E4B7C?style=for-the-badge)
![Reranking](https://img.shields.io/badge/Reranking-Cross--Encoder-FF6F61?style=for-the-badge)
![Eval](https://img.shields.io/badge/Eval%20Harness-Recall%40k%20%2B%20Statistical%20Significance-FFC107?style=for-the-badge)
![Providers](https://img.shields.io/badge/Providers-Anthropic%20%7C%20OpenAI%20%7C%20Ollama-412991?style=for-the-badge&logo=openai&logoColor=white)
![Observability](https://img.shields.io/badge/Observability-Cost%20%2B%20Latency%20Logging-00B2B1?style=for-the-badge)

- **Fully local & free by default:** embedded Qdrant + local embeddings + Ollama — no API key, no Docker, no model download needed to run the 232+ test suite (all green in CI).
- **Rigorous eval, not vibes:** a dedicated harness measures recall@k and keyword grounding, with bootstrap confidence intervals and McNemar tests for statistical significance — not just point estimates.
- **Honest experimentation:** ran Self-RAG, HyDE, and embedding-model comparisons as real experiments, and documented it when they *didn't* help (e.g. reranking measurably hurts recall@1 on this corpus, replicated on a second, independent one — reported as a finding, not hidden).
- **Extended to a real-world corpus:** beyond the synthetic demo, the platform now also serves a Turkish financial-fraud-awareness corpus sourced entirely from official government institutions (Emniyet Genel Müdürlüğü, SPK, İçişleri Bakanlığı, Ticaret Bakanlığı), with a hand-verified, grep-checked eval set — no fabricated content.

FastAPI · Qdrant · sentence-transformers · pytest · GitHub Actions CI.

#### 🤖 [NEXUS — Local AI Assistant](https://github.com/erturkeryavuz/NEXUS)

A local-first AI assistant platform: a modular, real-time agent system that keeps everything — inference, memory, tools — on-device.

![Local-First](https://img.shields.io/badge/Local--First-Privacy%20by%20Design-2E7D32?style=for-the-badge)
![Real-Time](https://img.shields.io/badge/Real--Time-WebSocket%20Agent%20States-4A90D9?style=for-the-badge)
![Agentic](https://img.shields.io/badge/Agentic-Tool%20Calling-8A2BE2?style=for-the-badge)
![Memory](https://img.shields.io/badge/Memory-Persistent%20(SQLite)-003B57?style=for-the-badge)

- **Backend:** Python, FastAPI, WebSockets, SQLite
- **Frontend:** React, TypeScript, Three.js (React Three Fiber)
- **AI:** Ollama local LLM inference, agentic tool calling
- **Tools:** calculator, file search/read, JSON/CSV analysis, restricted Python execution
- **Memory:** persistent conversational memory via SQLite
- **Real-time:** WebSocket-based agent states and a live activity timeline
- **Architecture:** modular and extensible — built to grow into RAG, voice, vision, and Git/GitHub tool integrations

---

### 🛠️ Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)

**Backend, Data & Frontend**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

**AI / ML**

![LLMs](https://img.shields.io/badge/LLMs-412991?style=for-the-badge&logo=openai&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge)
![NLP](https://img.shields.io/badge/NLP-FF6F61?style=for-the-badge)
![Prompt Engineering](https://img.shields.io/badge/Prompt%20Engineering-8A2BE2?style=for-the-badge)

**Tools & Platforms**

![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![SAP](https://img.shields.io/badge/SAP-0FAAFF?style=for-the-badge&logo=sap&logoColor=white)

---

### 🚀 Other Projects *(completed)*

- 🎓 **[FantasyBasketballApp](https://github.com/erturkeryavuz/fantasy-basketball)** — AI-driven fantasy basketball mobile app with LLM integration and live player stats. University graduation project.
- ⚽ **[Euro2024App](https://github.com/erturkeryavuz/Euro2024App)** — mobile app built around live tournament data.
- 🏀 **[NBASHOP](https://github.com/erturkeryavuz/NBASHOP)** — e-commerce concept app for NBA merchandise.
- 📈 **[TSLAIQ](https://github.com/erturkeryavuz/TSLAIQ)** — a prediction and alerting system for Tesla (TSLA) stock, generating signal-based alerts from market data.

---

### 📊 GitHub Stats

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=erturkeryavuz&color=brightgreen&label=Profile+Views" />
</p>
