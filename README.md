<div align="center">

# Guilherme Cavalcante

**AI-Augmented Engineer · LLMOps · Data Engineering · Cloud**

*Brasília, BR — open to remote*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/guilherme-cavalcante-dados/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/GscDtAnalytic)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:gui.cavalcante3o@gmail.com)

</div>

---

I build systems that put LLMs into production — from streaming data pipelines to eval infrastructure that catches prompt regressions before deploy.

Use Claude Code as an architecture amplifier: I define the system boundaries, own the decisions, and drive the execution.

---

## Projects

### [PromptBench Studio](https://github.com/GscDtAnalytic/PromptBench) — LLM Eval Infrastructure
> *LLM apps regress when prompts change without control. PromptBench treats prompts as versioned software assets.*

- `PromptVersion` is immutable — no UPDATE, every edit creates an auditable snapshot
- Measures quality, latency, variance, and **real cost** (tokens from the provider's `usage` response, not estimates)
- Regression verdict: **dimension ∧ slice ∧ cost** — a better global average doesn't earn promotion if any slice regresses
- 87% test coverage on the evaluation module; deterministic checks are pure functions

**Stack:** `Next.js` · `FastAPI` · `PostgreSQL 16` · `Redis` · `arq` · `Anthropic Claude`

---

### [Mapear-RN](https://github.com/GscDtAnalytic/Mapear-RN) — Political Intelligence Platform
> *Political opinion monitoring across 167 municipalities in Rio Grande do Norte, Brazil — at < R$5/month.*

- RSS + social media ingestion → NLP sentiment pipeline → LLM-generated strategic recommendations
- Real-time dashboard with RAG over regional political knowledge base
- Cloud-native on GCP with full data governance

**Stack:** `Python` · `GCP` · `BigQuery` · `dbt` · `Cloud Run`

---

### [Pulso](https://github.com/GscDtAnalytic/Pulso) — Real-time Crypto Intelligence
> *Exactly-once streaming pipeline with Claude as the anomaly explainer — ~US$40/month on GCP.*

- Redpanda → ksqlDB → Apache Iceberg with exactly-once semantics
- Claude explains detected anomalies in natural language, not just flags them
- Cost-controlled LLM integration with token tracking

**Stack:** `Redpanda` · `ksqlDB` · `Apache Iceberg` · `Python` · `Anthropic Claude`

---

## What I bring


---

## Approach

Every project here has:
- **A problem statement** — not just a stack demo
- **ADRs** (Architecture Decision Records) explaining why each key decision was made
- **A build audit trail** — `docs/progress/blockN.md` logging what was done, what ran, what was decided
- **Real numbers** — cost, latency, test coverage — not vague claims

---

## Certifications

`AWS Certified Cloud Practitioner` · `Microsoft Azure AI Essentials` · `Anthropic Claude 101` · `Anthropic Claude Code in Action`

---

## Currently building

- Expanding PromptBench with multi-model judge (majority vote), continuous eval on real traffic, and GitHub Actions PR gate
- Growing English fluency for international collaboration

---

<div align="center">

*"A better global average doesn't earn promotion when it breaks the cost budget."*  
— from PromptBench Studio's regression verdict

</div>
