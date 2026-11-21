# Ertürk Eryavuz

**AI Engineer & Python Backend Developer** · Istanbul, Turkey  
Computer Engineering graduate (Maltepe University, 2025) focused on **LLM/RAG systems, agent orchestration, deterministic workflow runtimes, and Python backend engineering**.

[LinkedIn](https://www.linkedin.com/in/erturkeryavuz) · [Email](mailto:erturkeryavuz@gmail.com) · [GitHub](https://github.com/erturkeryavuz)

**Quick Navigation:** [Featured AI Systems (Live Demos)](#featured-ai-systems--live-interactive-demos) · [Mobile Applications](#mobile-applications) · [Additional Repositories](#additional-repositories) · [Technical Stack](#technical-stack) · [Contact](#contact)

---

## Engineering Approach

I build local-first AI and backend systems around **predictability, explicit authorization boundaries, and inspectable evidence** — favoring verifiable retrieval, bounded tool execution, deterministic validation, and candid reporting of model limitations over opaque automation.

---

## Featured AI Systems — Live Interactive Demos

These three private, local-first AI systems are presented through **public, self-contained interactive showcases** on GitHub Pages. Each live site replays real recorded runs from its local runtime over synthetic or public benchmark data, with **no live browser-side inference and no external backend connection**, so reviewers can inspect plans, rankings, approvals, provenance records, and documented failure modes directly.

### 1. QUO · Conductor — Local AI Orchestration Runtime
**[→ Open Live Demo](https://erturkeryavuz.github.io/quo-conductor-demo/)** · [Demo Repository & Notes](https://github.com/erturkeryavuz/quo-conductor-demo) · `Status: Live Static Showcase (8 Recorded Runs)`

[![QUO Conductor overview showing planned workflows, authorization states, and execution timeline](https://erturkeryavuz.github.io/quo-conductor-demo/media/quo-01-overview.png)](https://erturkeryavuz.github.io/quo-conductor-demo/)

- **Plan-then-execute orchestration:** Routes simple questions directly and decomposes tool-requiring requests into dependency-ordered plans where each step runs through a declared capability with an effect class, permission policy, and time budget.
- **Mandatory write authorization:** Read-only capabilities run by policy, while workspace writes pause for explicit approval bound to the exact action digest; refusals and mid-run cancellations halt execution without invoking the tool.
- **Inspectable execution journal:** Reconstructs the interface, timeline, telemetry, and full payload log from a durable journal, while transparently documenting small local-model (`llama3.2:3b`) answer mistakes and scripted-client approval playback.
- **Publicly demonstrated capabilities:** Local LLM orchestration (`llama3.2:3b`), capability-scoped tool execution, approval/refusal/cancellation flows, durable journaling.

---

### 2. RAG Platform · Evidence Desk — Hybrid Retrieval & Cited Generation
**[→ Open Live Demo](https://erturkeryavuz.github.io/rag-evidence-desk-demo/)** · [Demo Repository & Notes](https://github.com/erturkeryavuz/rag-evidence-desk-demo) · `Status: Live Static Showcase (Synthetic Corpus & Benchmarks)`

[![RAG Platform Evidence Desk showing a cross-document cited answer traced directly to source passages](https://erturkeryavuz.github.io/rag-evidence-desk-demo/media/rag-03-featured-answer.png)](https://erturkeryavuz.github.io/rag-evidence-desk-demo/)

- **Hybrid retrieval with Reciprocal Rank Fusion:** Combines dense embeddings (`multilingual-e5-small`) and BM25 lexical search so both semantic questions and exact error codes (such as `PW-4107`) reach the top-five context window.
- **Citation tracing & refusal discipline:** Links every citation marker to the exact passage given to the model, runs deterministic marker-resolution checks alongside manual groundedness review, and refuses questions unsupported by the corpus.
- **Empirical reranker evaluation:** Benchmarks an optional cross-encoder reranker (`ms-marco-MiniLM-L-6-v2`) on labelled English (20 questions) and Turkish (21 questions) sets — keeping it disabled by default after measuring lower Recall@1 and higher latency, and publishing reviewed 3B-model failure cases openly.
- **Publicly demonstrated capabilities:** Dense + BM25 hybrid retrieval, RRF, cross-encoder evaluation, grounded citation inspection, 2D PCA corpus view, local Ollama generation (`llama3.2:3b`).

---

### 3. AI Enterprise Automation · Ledger — Governed Workflows & File Provenance
**[→ Open Live Demo](https://erturkeryavuz.github.io/aiea-ledger-demo/)** · [Demo Repository & Notes](https://github.com/erturkeryavuz/aiea-ledger-demo) · `Status: Live Static Showcase (26 Recorded Scenarios)`

[![AIEA Ledger showing the six-stage governed file lifecycle from blocked write to verified revision and drift detection](https://erturkeryavuz.github.io/aiea-ledger-demo/media/aiea-01-overview.png)](https://erturkeryavuz.github.io/aiea-ledger-demo/)

- **Strict pre-execution validation:** Rejects unknown keys or tools, duplicate IDs, dependency cycles, dangling references, and oversized requests before any step starts, then runs valid steps deterministically one at a time in dependency order.
- **High-risk step authorization & process isolation:** Blocks unapproved high-risk writes across both interactive terminal prompts and JSON contract mode, executing each tool call in a separate subprocess with an empty environment and supporting idempotent replay of identical requests.
- **SQLite provenance & external drift detection:** Records run history and SHA-256 artifact manifests so `verify`, `inspect`, and `prune` detect external file tampering (`content_mismatch`), missing/untracked files, and superseded revisions across 41 recorded CLI commands.
- **Publicly demonstrated capabilities:** Python CLI workflow runtime, DAG/schema validation, authorization gates, subprocess isolation, SQLite provenance tracking.

---

## Mobile Applications

Both projects have publicly available source repositories. Interactive, phone-framed web showcases are planned as upcoming portfolio milestones and are not yet published. Each summary reflects features verified in the available source code.

### Fantasy Basketball Platform
[Source Repository](https://github.com/erturkeryavuz/fantasy-basketball) · `Status: Public Source Code · Interactive Mobile Showcase Planned`

- **Full-stack graduation project (Maltepe University):** Combines a **Django + Django REST Framework** backend with a native **SwiftUI** iOS client.
- **Verified iOS & API workflows:** Token-authenticated registration and login, team and player directories, player detail cards across six rarity tiers (`Gold` through `DarkBlueDiamond`), a credit-based `PackMarket` with randomized card-pack opening (`POST /api/open-pack/`), and a personal `My Cards` inventory.
- **Backend league engine:** Implements relational Django models and REST endpoints for leagues, league membership, match schedules, result recording, player/team statistics, and league standings.
- **Stack:** Python · Django · Django REST Framework · SQLite · Swift · SwiftUI

### Euro2024App — Tournament Companion
[Source Repository](https://github.com/erturkeryavuz/Euro2024App) · `Status: Public Source Code · Interactive Mobile Showcase Planned`

- **Native iOS tournament viewer:** SwiftUI application built for browsing UEFA Euro 2024 fixtures, match detail timelines (goals and cards), group standings, team pages, and tournament news.
- **Multi-facet player explorer & user profile:** Includes a filterable player directory (filtering by position, country, and minimum rating) alongside Firebase Authentication, Firestore-backed user profiles, and favorite team/player/match selections.
- **Data ingestion pipeline:** Includes a Python Firebase Admin SDK script (`euro2024_matches.py`) that uploads structured match and event JSON datasets into nested Firestore collections.
- **Stack:** Swift · SwiftUI · Firebase (Auth, Firestore, Storage) · Python

---

## Additional Repositories

| Repository | Stack | Source-Verified Summary | Status |
|---|---|---|---|
| **[TSLAIQ](https://github.com/erturkeryavuz/TSLAIQ)** | Python, TensorFlow / Keras, pandas, scikit-learn, `yfinance`, `ta` | Financial time-series research pipeline ingesting historical TSLA data, engineering technical indicators (RSI, EMA20, EMA50, MACD, OBV), comparing baseline LSTM vs. attention-augmented LSTM checkpoints, and generating threshold-based CLI signals. | Research archive |
| **[NBASHOP](https://github.com/erturkeryavuz/NBASHOP)** | PHP, MySQL, Bootstrap, HTML/CSS, JavaScript | University coursework e-commerce storefront and PHP admin panel built on an EShopper Bootstrap template. | Coursework archive |

---

## Technical Stack

| Domain | Technologies & Practices |
|---|---|
| **Languages** | Python, TypeScript, Swift, JavaScript, SQL |
| **AI & LLM Systems** | Local LLMs (Ollama), RAG (Dense Embeddings, BM25, RRF, Cross-Encoder Reranking), Agent Orchestration, Groundedness & Retrieval Evaluation |
| **Backend & Data** | FastAPI, Django, Django REST Framework, SQLite, PostgreSQL, pandas, NumPy |
| **Frontend & Mobile** | SwiftUI, React, HTML5 / CSS3, Responsive Static Web Interfaces |
| **Engineering Practices** | Git, REST API Design, `pytest`, Deterministic Validation, Permission & Subprocess Boundaries |

---

## Contact

Open to **Junior / Early-Career AI Engineering, LLM/RAG, Agent Systems, and Python Backend** opportunities.

- **LinkedIn:** [linkedin.com/in/erturkeryavuz](https://www.linkedin.com/in/erturkeryavuz)
- **Email:** [erturkeryavuz@gmail.com](mailto:erturkeryavuz@gmail.com)
