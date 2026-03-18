<div align="center">

```
██████╗  ██████╗ ██████╗ ████████╗███████╗ ██████╗ ██╗     ██╗ ██████╗ 
██╔══██╗██╔═══██╗██╔══██╗╚══██╔══╝██╔════╝██╔═══██╗██║     ██║██╔═══██╗
██████╔╝██║   ██║██████╔╝   ██║   █████╗  ██║   ██║██║     ██║██║   ██║
██╔═══╝ ██║   ██║██╔══██╗   ██║   ██╔══╝  ██║   ██║██║     ██║██║   ██║
██║     ╚██████╔╝██║  ██║   ██║   ██║     ╚██████╔╝███████╗██║╚██████╔╝
╚═╝      ╚═════╝ ╚═╝  ╚═╝   ╚═╝   ╚═╝      ╚═════╝ ╚══════╝╚═╝ ╚═════╝ 
```

### AI / ML Engineer · LLM Systems · Eval-first Engineering

[![Portfolio](https://img.shields.io/badge/Portfolio-akanksha--th.github.io-orange?style=flat-square&logo=github)](https://akanksha-th.github.io/Portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-akanksha--thakur-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/akanksha--thakur)
[![Email](https://img.shields.io/badge/Email-akanksha.th.work%40gmail.com-red?style=flat-square&logo=gmail)](mailto:akanksha.th.work@gmail.com)
[![ICPR Paper](https://img.shields.io/badge/ICPR_2024-Published_Paper-green?style=flat-square&logo=googlescholar)](https://link.springer.com/chapter/10.1007/978-3-031-78166-7_21)

</div>

---

I build **production LLM systems** - not just demos. Eval layers, async pipelines, real observability. Aerospace Engineering grad who went deep on AI from year two, published at ICPR 2024, and has a strong bias for measuring everything I ship.

> *Most AI portfolios show you what someone built. This one shows you what it measured.*

---

## 🚢 Featured Project

### [`podcast_fact_extractor_rag`](https://github.com/akanksha-th/podcast_fact_extractor_rag) – Production Telegram Bot

> LangGraph · Qdrant · ARQ · Redis · DeepEval · Prometheus · Grafana · FastAPI · GitHub Actions

The one project that has everything: async ingestion, an eval layer, CI/CD with threshold gates, and observability dashboards. Built after a round-1 rejection where the interviewers cited gaps in LLM evaluation – so I went and built the eval framework myself.

| Component | What it does | Result |
|---|---|---|
| **Async Ingestion** | ARQ + Redis task queue for background audio processing | Concurrent session handling without blocking |
| **Eval Layer** | DeepEval golden dataset – faithfulness, answer relevancy, context precision | Caught **3 prompt regressions** pre-merge |
| **CI/CD Eval Gates** | GitHub Actions blocks merges below threshold scores | Zero regression deploys |
| **Observability** | Prometheus + Grafana – p95 latency, query throughput | Found & fixed **2× cold-start slowdown** |

---

## 📂 Projects

### [`youtube-sentiment-api`](https://github.com/akanksha-th) – Production Inference API
> FastAPI · RoBERTa · Redis · asyncio · PyTorch

- **Batch Inference:** FastAPI + RoBERTa pipeline – 100+ comments/request via async batching, **~40% lower latency** vs sequential
- **Response Caching:** Redis TTL caching reduces p95 from ~800ms to **<100ms** on cache hits  
- **Non-blocking Inference:** RoBERTa forward passes offloaded to thread pool via asyncio – no GIL contention

---

### [`slack-nl-to-sql`](https://github.com/akanksha-th) – LLM Application
> LangChain · FAISS · PostgreSQL · Slack API · FastAPI

- **NL Interface:** Schema-aware LangChain prompt chain translates plain-English questions into valid PostgreSQL – eliminates SQL for routine lookups
- **Semantic Schema Matching:** FAISS-embedded table/column metadata retrieves the most relevant schema context per query, reducing hallucinated column names

---

### [`TedTalk-Recommendation-System`](https://github.com/akanksha-th/TedTalk-Recommendation-System) – Semantic Search
> FAISS · HuggingFace · FastAPI · SQLite

- **Retrieval Engine:** 2,500+ TED Talk transcripts indexed as dense embeddings – full transcript matching, not just titles
- **REST API:** FastAPI endpoint with cosine similarity ranking over the full corpus

---

### [`Flight_Price_Prediction`](https://github.com/akanksha-th/Flight_Price_Prediction) – MLOps Pipeline
> ZenML · MLflow · Scikit-learn · Pandas

- End-to-end ML pipeline with experiment tracking (MLflow) and pipeline orchestration (ZenML)
- Feature engineering, model selection, and tracked experiments with reproducible runs

---

## 🔬 Research

**ASwin-YOLO: Attention–Swin Transformers in YOLOv7 for Air-to-Air UAV Detection**  
*ICPR 2024 – International Conference on Pattern Recognition*  
[→ Read Paper](https://link.springer.com/chapter/10.1007/978-3-031-78166-7_21)

Replaced the YOLOv7 backbone with a Swin Transformer + LSTM attention hybrid for aerial UAV detection:
- **54% reduction** in training time (2.2× faster)
- **5% accuracy gain** on benchmark
- Single-GPU training within one day

---

## 🛠 Stack

```
LLM / RAG     │ LangGraph · LangChain · FAISS · Qdrant · RAG architectures · Prompt engineering
Evaluation    │ DeepEval · Golden dataset design · CI eval gates · Faithfulness · Context precision
ML / DL       │ PyTorch · HuggingFace Transformers · Scikit-learn · YOLOv7 · RoBERTa · Swin Transformer  
Backend       │ FastAPI · Redis · ARQ · asyncio · PostgreSQL · REST APIs
MLOps         │ Docker · Prometheus · Grafana · GitHub Actions · ZenML · MLflow · structlog
Languages     │ Python (primary) · SQL · Bash
```

---

## 📄 Experience

**Research Trainee – CSIR-CSIO, Chandigarh** *(Jan 2024 - Jul 2024)*  
Computer Vision research on transformer-based object detection. Co-authored paper published at ICPR 2024.

**B.Tech Aerospace Engineering – PEC University of Technology** *(2021 - 2025, GPA: 7.9)*  
Non-traditional path into AI: independent deep-dive into ML/DL from year two, building production systems outside coursework.

---

<div align="center">

**Open to AI Engineering and Data Science roles in India.**  
Teams that care about eval, observability, and shipping things that actually work.

[akanksha.th.work@gmail.com](mailto:akanksha.th.work@gmail.com)

</div>
