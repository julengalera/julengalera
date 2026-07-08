# Julen Galera · Senior Full-Stack Engineer

**TypeScript / React / Node / AWS · Booking & transactional systems · Production LLM/RAG**

I build systems where correctness is money: booking platforms where a race condition means a double-booked hotel room, and AI products where a wrong citation means a legal problem.

- **4+ years at EY:** engineering the central reservations platform of one of the world's largest hotel chains (530+ properties, 56 countries). Monolith → microservices, multi-currency, high availability.
- **Founder of [Ploma](https://ploma.es):** an AI copilot for Spanish building regulations. Designed, built and operated solo, from corpus ingestion to production infrastructure and billing.

---

## Featured work

### 🏨 Global booking platform (EY, enterprise client)

Migration of booking-critical B2B reservation flows from a legacy monolith to independently deployable services, in a platform running across 56 markets.

- Complete modules built end to end: Spring Boot APIs + Vue/Nuxt frontends
- Designed and implemented the API of a corporate events & group reservation system used by enterprise clients
- Daily contact with what makes this domain hard: live inventory, overbooking rules, channel managers, multi-currency pricing

*Code is proprietary. An architecture case study (decisions, trade-offs, diagrams) is on its way. Ask me about it.*

### 🤖 Ploma: production RAG that cites the law, verbatim

Spanish architects must legally justify building-code compliance against a 2,000+ page corpus. Generic LLMs hallucinate regulations; in compliance, "probably right" is worthless. Ploma answers regulatory queries and generates technical reports with **verifiable, article-level citations**.

Architecture highlights:

- **Hybrid retrieval:** pgvector + BM25/full-text fused with Reciprocal Rank Fusion, hierarchical chunk expansion (parent/child/sibling) and cross-references
- **Multi-model orchestration:** a lightweight classifier routes every query (model, depth, retrieval strategy) before spending expensive tokens
- **Agentic RAG:** the LLM pulls terminology, official ministry commentary and previously seen chunks on demand via tools
- **Quality loop:** an async auditor scores every answer post-stream against hallucination and failure modes; every interaction is captured for future fine-tuning
- **Resilience:** per-provider circuit breakers (Anthropic, OpenAI, Cohere) with shared state and active probing
- **Business layer:** Stripe subscriptions and usage gating from day one

**Stack:** TypeScript · Next.js · React · Supabase (Postgres + pgvector) · AWS Bedrock (Claude) · ECS Fargate · Cohere · Stripe · Docker

---

## How I work

Small PRs, strict types (`strict`, `noUncheckedIndexedAccess`), tests where they pay for themselves, clean commit history, and documentation the next engineer will thank you for. In contracting you're judged by your diff, so I write mine accordingly.

## Stack

- **Backend:** Node.js, Fastify, Java 21, Spring Boot 3, PostgreSQL, Redis, REST APIs, microservices
- **Frontend:** React 19, Next.js, Vue/Nuxt, TypeScript, Tailwind, shadcn/ui
- **AI/LLM:** Claude (AWS Bedrock), OpenAI embeddings, hybrid RAG (pgvector + BM25 + RRF), Cohere Rerank, agentic tool use, multi-model orchestration
- **Cloud & delivery:** AWS (ECS Fargate, RDS, ElastiCache, S3, CloudWatch, Bedrock), Terraform, Docker, GitHub Actions, Vercel

---

## Availability

✅ **Available for B2B contracts.** Remote, based in Madrid (CET), full UK/EU overlap. Fluent English & Spanish.

Best fit: backend or full-stack contract work with teams in 🇬🇧 UK, 🇳🇱 Netherlands, 🇩🇪 Germany, or remote-first companies anywhere. Especially booking/transactional platforms and production LLM features.

[LinkedIn](https://linkedin.com/in/julengalera) · [julen.galera.dev@gmail.com](mailto:julen.galera.dev@gmail.com) · [ploma.es](https://ploma.es)
