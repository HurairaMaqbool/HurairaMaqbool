<div align="center">

```
██╗  ██╗██╗   ██╗██████╗  █████╗ ██╗██████╗  █████╗ 
██║  ██║██║   ██║██╔══██╗██╔══██╗██║██╔══██╗██╔══██╗
███████║██║   ██║██████╔╝███████║██║██████╔╝███████║
██╔══██║██║   ██║██╔══██╗██╔══██║██║██╔══██╗██╔══██║
██║  ██║╚██████╔╝██║  ██║██║  ██║██║██║  ██║██║  ██║
╚═╝  ╚═╝ ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝╚═╝  ╚═╝╚═╝  ╚═╝
```

### AI Engineer · LangChain · LangGraph · Multi-Agent Systems · RAG

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/huraira-maqbool-b696a5277)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hurairac37@gmail.com)
[![Fiverr](https://img.shields.io/badge/Fiverr-1DBF73?style=for-the-badge&logo=fiverr&logoColor=white)](https://fiverr.com/huraira_maqbool)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HurairaMaqbool)

</div>

---

## 🧠 About Me

I build **production-grade AI systems** — from multi-agent pipelines to RAG architectures and conversational AI.
My focus is on systems that actually work in the real world: reliable, fast, and deployable.

- 🔭 Currently building: **Multi-Agent AI systems** with LangGraph + CrewAI
- ⚡ Speciality: **Hybrid RAG** (FAISS + BM25), agentic workflows, LLM integration
- 🌍 Open to: **Remote AI Engineering roles & freelance projects**
- 📫 Reach me: **hurairac37@gmail.com**

---

## 🛠️ Tech Stack

**AI/LLM Frameworks**
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-FF6B35?style=flat-square&logoColor=white)
![CrewAI](https://img.shields.io/badge/CrewAI-6C3483?style=flat-square&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**Vector Databases & Search**
![FAISS](https://img.shields.io/badge/FAISS-0057B7?style=flat-square&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF4500?style=flat-square&logoColor=white)
![BM25](https://img.shields.io/badge/BM25_Hybrid_Search-2ECC71?style=flat-square&logoColor=white)

**LLM Providers**
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)

**Backend & Deployment**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

---

## 🚀 Featured Projects

### 🧭 [CodeNavigator — Agentic Graph-Augmented RAG for Codebase Onboarding](https://github.com/HurairaMaqbool/CodeNavigator)
> Agentic RAG platform that ingests any Git repository, builds a triple index (dense embeddings + BM25 keyword + NetworkX call graph), and answers codebase questions through a deterministic FSM agent — every claim runs through a multi-layer verification firewall against the real file system, AST, and call graph before it's shown to you.

`FastAPI` `Next.js` `ChromaDB` `BM25` `NetworkX` `Tree-sitter` `Groq` `PostgreSQL` `RAGAS` `Python`

**Key highlights:**
- 🔄 Deterministic FSM agent loop — `PLAN → ACT → OBSERVE → DECIDE → VERIFY → RESPOND` — not a free-form agent
- 🕸️ Graph-augmented retrieval — NetworkX call graph with BFS-proximity ranking for caller/callee traversal
- 🛡️ Multi-layer verification firewall — structural, AST, and relationship grounding checks; hallucinated claims are blocked, not softened
- 🔀 Hybrid retrieval — ChromaDB + BM25 fused via Reciprocal Rank Fusion (RRF)
- 📊 Auto-generates Mermaid call-graph diagrams rendered live in the Architecture Explorer
- 🧪 Built-in RAGAS evaluation dashboard — every run tracked, including scores below target, not just a single flattering number

**Verified metrics (from the live evaluation dashboard):**
- 27/27 (100%) on the canonical adversarial suite — 0% hallucinations, 0% unexplained abstentions
- 10/10 (100%) golden-set CI pass rate
- 703 passed / 13 failed / 9 skipped across the full test suite
- RAGAS faithfulness 0.55–0.59 and context recall ~0.49 — below the 0.70 target and actively being tuned, tracked transparently run-over-run

🔗 Repo: https://github.com/HurairaMaqbool/CodeNavigator

---

### 🛡️ [ThreatMind — Autonomous Cyber Threat Intelligence Pipeline](https://github.com/HurairaMaqbool/ThreatMind)
> 11-agent LangGraph pipeline that autonomously monitors security blogs and advisories, decides what's actually worth hunting for, and turns it into validated, multi-platform SIEM detections — running as a standing service with a live scheduler, not a one-off script.

`LangGraph` `Groq` `ChromaDB` `FastAPI` `Streamlit` `pySigma` `Docker` `Python`

**Key highlights:**
- 🔗 11-stage pipeline — Triage → Discovery → Extraction → Threat Intel → Coverage Planner → RAG → Reasoning → KQL Generator → Validator (retry loop) → Coverage Critic → Report
- 🧭 Dedicated Coverage Planner decides *what* to detect (behavioral vs. tool-artifact vs. indicator-only) before any query is generated, prioritizing detections that are hard for attackers to evade
- 📚 RAG-grounded generation — retrieval against an authoritative Sentinel/Defender schema via ChromaDB, plus historical KQL and similar past threats for context
- 🛠️ Self-correcting validator — auto-fixes known wrong-but-plausible column names (e.g. `CommandLine` → `ProcessCommandLine`) against the real schema before re-scoring
- 🌐 Multi-platform output — validated KQL converts to Sigma, then to Splunk, QRadar, Elasticsearch, CrowdStrike, Wazuh, and SentinelOne
- ⏰ Live scheduler crawls 10 threat-intel feeds on an interval, dedupes seen articles via ChromaDB, and pushes Slack/email alerts for HIGH/CRITICAL findings
- 🖥️ REST API (FastAPI) + 5-page Streamlit SOC dashboard, deployable via Docker Compose

Built in collaboration with Ahmad Shabbir.

🔗 Repo: https://github.com/HurairaMaqbool/ThreatMind

---

### 🤖 [Aria — Bilingual AI Personal Assistant](https://github.com/HurairaMaqbool/aria-ai-assistant)
> LangGraph-powered conversational agent with persistent memory, real-time web search, and Urdu/English bilingual support.

`LangGraph` `ChromaDB` `Groq` `Streamlit` `DuckDuckGo API` `Python`

**Key highlights:**
- 🧠 Persistent memory via ChromaDB vector store
- 🌍 Auto-detects Urdu & English — responds in same language
- ⚡ Ultra-fast inference with Groq (Llama 3.3 / Mixtral)
- ✅ Task management + math solver + live web search

**Verified metrics:** 4.00/5.0 RAGAS eval score · 43 CI tests passing · $0.00244 avg cost/query

🔗 Live Demo: https://aria-ai-assistant-axw5b3axeeyofyshudo2qe.streamlit.app/?uid=user_cf092c53
🔗 Repo: https://github.com/HurairaMaqbool/aria-ai-assistant

---

### 🔍 [NexusRAG — Bilingual Hybrid RAG Engine](https://github.com/HurairaMaqbool/NexusRAG)
> Multi-tool RAG agent with hybrid (semantic + keyword) retrieval, bilingual Urdu/English support, and persistent memory — deployed as a live Streamlit app.

`LangChain` `LangGraph` `FAISS` `BM25` `ChromaDB` `Groq` `Streamlit` `FastAPI` `Sentence Transformers` `Python`

**Key highlights:**
- 📄 Ingests PDF, DOCX, TXT — chunked + embedded automatically
- 🔍 Hybrid retrieval: FAISS (semantic) + BM25 (keyword) ensemble for higher accuracy
- 🌐 Bilingual support — handles queries and responses in Urdu and English
- 🧠 Persistent conversation memory via ChromaDB + LangGraph state management
- 🧮 Built-in calculator and DuckDuckGo web search tools
- ⚡ Production architecture — FastAPI backend, deployed live on Streamlit Cloud

🔗 Live Demo: https://ai-rag-agent-8vfrcjngsjtppsrm2appwsc.streamlit.app/
🔗 Repo: https://github.com/HurairaMaqbool/NexusRAG

---

### 📚 [LMS AI Chatbot](https://github.com/HurairaMaqbool/LMS-CHATBOOT)
> Full-stack AI assistant for students, teachers & admins — natural language access to marks, attendance & assignments.

`Node.js` `React.js` `Groq API` `Socket.IO` `JWT` `Redis` `Bull Queues` `FastAPI`

**Key highlights:**
- 🎓 Role-based access — Student / Teacher / Admin
- 🧠 AI intent classification & smart query routing
- ⚡ Real-time notifications via Socket.IO
- 📊 Automated attendance warnings & broadcast messaging
- 🔐 JWT auth + RBAC secure API design

🔗 Repo: https://github.com/HurairaMaqbool/LMS-CHATBOOT

---

## 📊 GitHub Stats

<div align="center">

![Huraira's GitHub Stats](https://github-readme-stats.vercel.app/api?username=HurairaMaqbool&show_icons=true&theme=tokyonight&hide_border=true&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=HurairaMaqbool&layout=compact&theme=tokyonight&hide_border=true)

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=HurairaMaqbool&theme=tokyonight&hide_border=true)

</div>

---

## 🏅 Certifications

| Issuer | Certification |
|--------|--------------|
| 🟦 NVIDIA | AI/Deep Learning Fundamentals |
| 🤗 HuggingFace | NLP & Transformers |
| 🪟 Microsoft | Azure AI Fundamentals |
| 🤖 Anthropic | Claude AI Development |

---

## 🌱 Currently Exploring

```
Multi-Agent Orchestration  →  LangGraph + CrewAI
Production RAG Evaluation  →  RAGAS Framework
LLM Fine-tuning            →  LoRA / QLoRA
Cloud Deployment           →  Docker + CI/CD Pipelines
```

---

<div align="center">

**Open for remote AI Engineering roles & freelance projects**
📧 hurairac37@gmail.com

![Profile Views](https://komarev.com/ghpvc/?username=HurairaMaqbool&color=blueviolet&style=flat-square)

</div>
