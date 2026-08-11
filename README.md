<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/convergence-dark.svg">
  <img src="assets/convergence-light.svg" width="100%" alt="Two strands — neural networks from 2020 and backend from 2022 — converging into a single line by 2026">
</picture>

### Marcus Vinicius — *Chuck*

Backend engineer at [@Samplemed](https://github.com/Samplemed). I build Python services — FastAPI, Django, Postgres, Redis — and reach for Rust when latency is the whole point.

I came to programming for neural networks and stayed for the backend. Lately the two have met again: most of what I build now has a model somewhere in the pipeline.

---

#### Selected work

- **[webhook-ingester](https://github.com/Pissinatti-py/webhook-ingester)** `Rust` — HMAC verification, dedup and enqueue in a single atomic Lua script. **14k req/s** on the bundled stress test, so provider retry storms never reach the app server.
- **[finance-ai-assistant](https://github.com/Pissinatti-py/finance-ai-assistant)** `Python` — LangGraph agent with tools, RAG and a semantic cache over Postgres/pgvector. Embeddings run locally on CPU, so the vector side needs no second vendor.
- **[market-insights-service](https://github.com/Pissinatti-py/market-insights-service)** `Python` — Celery collectors → Postgres → curation by a self-hosted LLM. Idempotent end to end: every row carries a `dedup_key` and upserts with `ON CONFLICT DO NOTHING`.
- **[fastapi-observability-demo](https://github.com/Pissinatti-py/fastapi-observability-demo)** `Python` — Job progress streamed live over SSE, every request and job instrumented with Prometheus and rendered in Grafana.
- **[fastapi-boilerplate](https://github.com/Pissinatti-py/fastapi-boilerplate)** `Python` — The base the services above inherit: async SQLAlchemy 2.0, Alembic, Docker, clean layering.
- **[portfolio](https://github.com/Pissinatti-py/portfolio)** `Vue 3 · TypeScript` — My site, at [pissinatti-py.github.io/portfolio](https://pissinatti-py.github.io/portfolio/). Sidebar shell with a command palette and scroll-driven animation built on the Intersection Observer — no animation library.

#### Where I started — [@Chuckpy](https://github.com/Chuckpy)

My first account, still online. Django apps and machine-learning experiments from 2020–2022, back when I was learning both at once.

- **[Django-ecommerce](https://github.com/Chuckpy/Django-ecommerce)** ⭐5 — Full storefront built on Django; my most-starred project.
- **[Management-Sistem](https://github.com/Chuckpy/Management-Sistem)** ⭐3 — Django + Bootstrap system for managing and organising records.
- **[SOM_suspicious-credit-activity](https://github.com/Chuckpy/SOM_suspicious-credit-activity)** — Self-organising map that ranks credit applicants by how suspicious their activity looks.
- **[python-monopoly](https://github.com/Chuckpy/python-monopoly)** — Monopoly simulator in pure standard-library Python, run over many trials to compare player strategies.

---

#### What I'm working on

| | |
|---|---|
| **Building** | `market-insights-service` — market signals collected, deduplicated and curated by a local LLM |
| **Maintaining** | `fastapi-boilerplate` and `auth-boilerplate`, the scaffolding everything else sits on |
| **Exploring** | Rust on latency-critical paths · LLM agents that run without a cloud vendor |
| **Working** | Sample360 at [@Samplemed](https://github.com/Samplemed) — a multi-tenant health platform on Django + Vue 3 |

#### Stack

```
Languages   Python · Rust · TypeScript
Backend     FastAPI · Django / DRF · SQLAlchemy 2.0 (async) · Celery · axum
Data        PostgreSQL · pgvector · Redis
Ops         Docker · GitHub Actions · Prometheus · Grafana · uv
AI          LangGraph · Anthropic API · Ollama · RAG · semantic caching
```

---

[Portfolio](https://pissinatti-py.github.io/portfolio/) · [LinkedIn](https://www.linkedin.com/in/marcusviniciusfonsecap) · [marcusandrade.37@gmail.com](mailto:marcusandrade.37@gmail.com)
