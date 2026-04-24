<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=200&section=header&text=Sameer%20Shaik&fontSize=60&fontColor=ffffff&fontAlignY=35&desc=Full%20Stack%20AI%20Engineer%20%7C%20Agent%20Systems%20%7C%20LLM%20Pipelines&descAlignY=55&descSize=18" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sameer-shaik6411/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SameerShaik786)
[![LeetCode](https://img.shields.io/badge/LeetCode_450+-FFA116?style=for-the-badge&logo=leetcode&logoColor=white)](https://leetcode.com/u/ShaikSameer_6411/)

<br/>

</div>

---

## 🧠 Who I Am

```python
class SameerShaik:
    name       = "Sameer Shaik"
    role       = "Full Stack AI Engineer"
    university = "RGUKT Nuzvid — B.Tech CSE (2023–Present)"
    cgpa       = 9.0
    location   = "Andhra Pradesh, India"

    focus = [
        "Multi-agent LLM systems",
        "Retrieval pipelines & evaluation harnesses",
        "End-to-end AI product development",
        "Finance-domain AI applications",
    ]

    philosophy = "I don't just integrate APIs. I think about architecture."
```

I'm a 3rd year CS student who builds full-stack AI products completely solo — from the agent pipeline and backend API to the database and frontend. My projects aren't tutorials or clones. They are real systems with real architectural decisions.

---

## 🚀 Projects

### 🔴 Stock Debate Analysis System
> *Four AI agents debate a stock. One verdict.*

A full-stack AI platform where **Bull**, **Bear**, **Neutral**, and **Judge** agents engage in a structured sequential debate over a stock ticker using real market data — producing an explainable **BUY / SELL / HOLD** verdict with a confidence score and source citations.

**What makes it different:** The agents don't just retrieve facts — they build arguments, challenge each other's reasoning, and the Judge synthesizes contradictions into a final decision. Real financial data from yfinance and Alpha Vantage. Streamed live to the frontend via WebSockets.

![LangGraph](https://img.shields.io/badge/LangGraph-000000?style=flat-square&logo=python&logoColor=white)
![GPT-4o](https://img.shields.io/badge/GPT--4o-412991?style=flat-square&logo=openai&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)

[→ View Repository](https://github.com/SameerShaik786/stock-debate-analysis)

---

### ⚙️ IdeaEvaluator — Startup Evaluation Workflow System
> *7 AI agents. Parallel execution. Deterministic scoring.*

A multi-agent intelligence platform that evaluates startups across **7 domains** — Financial Health, Market Potential, Competition, Risk, Longevity, Validation, and Investor Fit — in a dependency-aware pipeline.

**Key architectural decision:** The LLM is completely removed from the scoring step. Early versions had inconsistent scores because the LLM would hallucinate numbers. The final score is computed by a **deterministic weighted engine** — Financial 30%, Risk inverted 30%, Market 20%, Validation 20%. The agents only produce structured JSON. The math is pure Python.

Agents run in **3 waves using asyncio.gather** — Validator first sequentially, then Financial/Market/Competition in parallel, then Risk/Longevity/InvestorFit in a second parallel wave with upstream context merged in.

![AutoGen](https://img.shields.io/badge/AutoGen_v0.7-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![Groq](https://img.shields.io/badge/Groq_Llama3.3_70B-FF6B35?style=flat-square&logo=groq&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)

[→ View Repository](https://github.com/SameerShaik786/startup-idea-evaluator) · [→ Watch Demo](https://drive.google.com/file/d/1yI1juQjA_SIklLRudTsfTPczkfnGHSVK/view?usp=drive_link)

---

### 🔨 Code0 — Prompt to Live React App
> *Type a prompt. Get a running app.*

An AI application generator that converts natural language into working React applications — end to end. The agent generates code, writes files, runs terminal commands, and streams the live app from an **E2B cloud sandbox** in real time.

**What's hard about it:** Handling concurrent user sessions where each session has its own isolated sandbox environment. Inngest manages the event-driven workflow so agent failures don't crash other sessions.

![Gemini](https://img.shields.io/badge/Gemini_LLM-4285F4?style=flat-square&logo=google&logoColor=white)
![Inngest](https://img.shields.io/badge/Inngest-000000?style=flat-square&logo=inngest&logoColor=white)
![E2B](https://img.shields.io/badge/E2B_Sandbox-FF4500?style=flat-square&logo=e2b&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)

[→ View Repository](https://github.com/SameerShaik786/v0-clone) · [→ Live Demo](https://code-not-nine.vercel.app)

---

### 🧩 ClientPilot — AI-Powered Project Management
> *Raw client chaos → structured deliverables.*

A freelance project management platform with an **AI Scope Agent** that transforms unstructured client inputs — emails, Slack messages, meeting notes — into structured project deliverables.

**What's interesting:** Every LLM interaction is logged via `AgentRun` / `StepRun` models with inputs, outputs, and latency. This is an observability layer for AI — you can debug exactly why the agent produced a specific output and benchmark quality over time.

![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_LLM-4285F4?style=flat-square&logo=google&logoColor=white)
![React](https://img.shields.io/badge/React.js-61DAFB?style=flat-square&logo=react&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)

[→ View Repository](https://github.com/SameerShaik786/client-pilot)

---

## 🛠️ Tech Stack

<div align="center">

### Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### AI / Agent Stack
![LangGraph](https://img.shields.io/badge/LangGraph-000000?style=for-the-badge&logo=python&logoColor=white)
![AutoGen](https://img.shields.io/badge/AutoGen-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=for-the-badge&logo=pinecone&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)

### Backend
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)

### Frontend
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

### Databases & Infrastructure
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=SameerShaik786&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=6C63FF&icon_color=6C63FF&text_color=ffffff" width="48%" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=SameerShaik786&theme=tokyonight&hide_border=true&background=0d1117&ring=6C63FF&fire=6C63FF&currStreakLabel=6C63FF" width="48%" />

<br/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SameerShaik786&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=6C63FF&text_color=ffffff" width="40%" />

</div>

---

## 🏆 By The Numbers

<div align="center">

| 🤖 AI Projects Shipped Solo | 💻 LeetCode Problems | 🎓 CGPA | 📍 Year |
|:---:|:---:|:---:|:---:|
| 4 | 450+ | 9.0 | 3rd Year, RGUKT |

</div>

---

## 📬 Let's Connect

<div align="center">

I'm always open to interesting AI work, collabs, or just talking about agent systems.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Let's_Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sameer-shaik6411/)
[![Email](https://img.shields.io/badge/Phone-+91_6300622373-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](tel:+916300622373)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=100&section=footer" />

</div>
