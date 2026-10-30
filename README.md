## Saba Tandilashvili

AI engineer and founder of [Omio Labs](https://omiolabs.ge) in Tbilisi. I build AI products end to end,
from the model and the data to the interface, the server and the first paying customer, and I run them
in production myself.

### Featured: [Investigation Engine](https://github.com/sabatandilashvili/upgaming-project)

An agentic RAG system that answers questions across 62,000 documents with a report where every
sentence is checked against its sources. It finds where sources disagree and says "not established"
when the evidence isn't there. [Try it live](https://130-61-72-51.sslip.io).

| | |
|---|---|
| Held-out questions, never used for tuning | **14 / 14** |
| 95-question evaluation (Opus 5.5) | **0.958** correct |
| Prompt-injection attacks resisted | **14 / 14** |
| Cost per question | about **$0.09** |

Hybrid search (own BM25 + RRF on Postgres/pgvector), Claude tool use, a deterministic verifier,
Langfuse tracing, 85 tests in CI. Full method and failure analysis in
[EVALUATION.md](https://github.com/sabatandilashvili/upgaming-project/blob/main/EVALUATION.md).

### Products I've built and run

| | |
|---|---|
| **[HSAI](https://app.hsai.app)** | Health and safety compliance SaaS for Georgian companies. RAG assistant on Georgian law, AI-generated safety documents, payments, contractor management for enterprise clients. |
| **[BAZA](https://bazahub.ge)** | Sales-training academy for a client: staff practise sales calls with an AI buyer. |
| **[EVACMAP](https://evac.hsai.app)** | Turns an architect's CAD floor plan into a printable evacuation map: geometry extraction, room detection, route finding. |
| **[TRAILS.GE](https://trails.ge)** | Georgian hiking platform. |
| **[VANTIS](https://vantis.ge)** | Financial control for off-plan property developers. |

The source for these is private; [omiolabs.ge](https://omiolabs.ge) shows each one.

### Stack

Python (Flask, FastAPI) · TypeScript, React · PostgreSQL, pgvector · Claude, OpenAI, Gemini ·
RAG, agents, tool use, evals · Langfuse · Linux servers, nginx, systemd · GitHub Actions
