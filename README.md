# 👋 Hey, I'm Julen

Backend-heavy Software Engineer with 3+ years at **EY** building microservices for a global hotel booking platform (530+ properties, 56 countries). Currently building **Ploma**, a B2B SaaS that uses AI to generate regulatory compliance reports for architects.

I design and ship production systems end-to-end, from distributed backends to LLM-powered pipelines. Available for freelance contracts with international teams.

---

## 💡 About Me
- 🎓 **Computer Engineering** – UPC (Polytechnic University of Catalonia)
- 💼 **3+ years at EY** – Migrating a monolithic booking platform to microservices (Java 21, Spring Boot 3, AWS, 56 countries)
- 🚀 **Currently Building** – [Ploma](https://ploma.es) (AI-powered compliance SaaS), solo founder & full-stack engineer
- 🛠️ **Core Stack** – Java, Spring Boot, TypeScript, Next.js, PostgreSQL, AWS, LLM orchestration
- 🎯 **Focus** – Backend architecture, distributed systems, AI/LLM engineering, system design

---

## 🧠 Tech Stack

**Backend & Architecture:**
Java 21, Spring Boot 3, TypeScript, Node.js, Fastify, Next.js 16, Microservices, REST APIs, API Gateway, PostgreSQL, Redis, Supabase (RLS + pgvector), Hibernate/JPA, Flyway, streaming (NDJSON), circuit breakers

**AI & LLM Engineering:**
Claude Opus/Sonnet/Haiku (via AWS Bedrock), OpenAI Embeddings, RAG (hybrid vector + BM25/FTS + RRF), Cohere Rerank, pgvector, agentic tool use, prompt engineering, multi-model orchestration

**Frontend:**
React 19, Vue.js, Nuxt.js, Tailwind CSS, TypeScript, Server Components, shadcn/ui

**Cloud & DevOps:**
AWS (ECS Fargate, ECR, ALB, Bedrock, RDS, ElastiCache, S3, CloudWatch), Terraform, Vercel, Docker, GitHub Actions, CI/CD

**Payments & Billing:**
Stripe (subscriptions, one-off packs, webhooks, portal)

---

## 🚀 Featured Project: Ploma

**AI-Powered Technical Compliance Reports for Spanish Architects**

A full-stack B2B SaaS that generates *memorias técnicas*, the legal documents architects must submit to prove their building projects comply with the CTE (Código Técnico de la Edificación). Built solo from corpus ingestion to production deployment.

**RAG & AI Pipeline:**
- ✅ **Normative Corpus** – 9 DBs of Spanish building code (PDF → Markdown → enriched chunks → pgvector embeddings)
- ✅ **Hybrid Retrieval** – Vector search + BM25/FTS with Reciprocal Rank Fusion, hierarchical expansion (parent/child/sibling), cross-references
- ✅ **Multi-Model Router** – Intelligent classifier (3 parallel Haiku sub-calls) decides archetype, model, depth, and retrieval strategy per query
- ✅ **Agentic RAG** – Tools for terminology (Anejo A), official comments, and chunk recall. LLM fetches on demand via manifests
- ✅ **Cohere Rerank** – Cross-encoder scoring with per-subquery reranking and star-threshold selection
- ✅ **Dynamic Cap** – Kneedle elbow detection + marginal utility + coverage floor, replaces fixed token caps
- ✅ **Conversational Memory** – Rolling thread summary + chunk recall manifest + anti-ambiguity continuation, verified live

**Report Generator:**
- ✅ **Rule-Based Index Engine** – YAML rules decide which sections apply to each project (use, geometry, location)
- ✅ **Opus 4.7 Redactor** – Generates normative justifications citing retrieved chunks with strict tool use
- ✅ **Warning System** – LLM-detected inconsistencies, missing data, potential non-compliance

**Chat Consultant:**
- ✅ **Multi-Pregunta Fan-Out** – Parallel retrieval per sub-question with Jaccard clustering
- ✅ **4-Level Post-Retrieval Filter** – Haiku categorizes chunks as CRITICO/CONTEXTO/TANGENCIAL/BASURA
- ✅ **Anti-Sycophancy** – Evidence-first verification, anti-hallucination guardrails, Path C for accusations
- ✅ **Silent Auditor** – Post-stream Haiku audit on 5 dimensions + 9 failure modes (async worker)
- ✅ **Multimodal** – Figures from normative documents served as images to the LLM

**Infrastructure:**
- ✅ **Chat API** – Standalone Fastify service on ECS Fargate (eu-south-2), ALB + custom domain (api.ploma.es)
- ✅ **Circuit Breaker** – Per-provider (Anthropic, OpenAI, Cohere) with shared state in Supabase + active probing
- ✅ **Billing** – Stripe integration (subscription tiers + one-off packs), daily token budget gating
- ✅ **Dataset Flywheel** – Every generation/chat/audit captured for future fine-tuning, fail-safe, never blocks main flow

**Stack:**
TypeScript, Next.js 16, React 19, Tailwind 4, Supabase (Postgres + pgvector), AWS Bedrock (Claude), ECS Fargate, Cohere, OpenAI Embeddings, Stripe, Docker

---

## 📈 What I'm Working On

- **Backend Architecture** – Microservices, API design, distributed caching, transactional boundaries, DDD patterns
- **System Design** – Modular monolith → microservices extraction, API gateway design, blue/green deployments
- **LLM Systems at Scale** – Multi-model orchestration, prompt caching, cost/quality tradeoffs in production RAG
- **Enterprise RAG** – Hybrid retrieval (vector + lexical + RRF), dynamic context selection, agentic tool use
- **Infrastructure** – ECS auto-scaling, circuit breakers, Terraform, container orchestration, streaming APIs

**Not just prototyping. Shipping production systems that handle real scale and real compliance.**

---

## 📊 GitHub Stats

<img src="https://github-readme-stats.vercel.app/api?username=julengalera&show_icons=true&theme=tokyonight" height="160px"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=julengalera&layout=compact&theme=tokyonight" height="160px"/>

---

## 💼 Available for Freelance

I take on freelance contracts for backend engineering, AI/LLM integration, and system design. Based in Spain (CET), fluent in English and Spanish, experienced working with distributed international teams.

**What I can help with:**
- Backend architecture & API design (Java/Spring Boot or TypeScript/Node.js)
- LLM-powered features: RAG pipelines, multi-model orchestration, production AI systems
- System design & infrastructure (AWS, Terraform, containerized deployments)
- Migrating monoliths to microservices

**Ideal engagement:** contract/freelance with teams in 🇩🇪 Germany, 🇬🇧 UK, 🇺🇸 USA, or remote-first companies. Happy to work async across timezones.

---

## 🤝 Let's Connect

[LinkedIn](https://linkedin.com/in/julengalera) · [Email](mailto:julen.galera.dev@gmail.com) · [Ploma](https://ploma.es)

**Open to freelance contracts.** Backend-heavy, AI/LLM engineering, or senior full-stack roles with international teams.