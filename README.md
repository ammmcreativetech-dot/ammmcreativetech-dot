# Amos Matzke

**GEO / AI-Search Engineer · Full-Stack (Next.js + AI/RAG)**
Founder, AM Creative Tech UG · Founder & Lead Architect of [quanta-study.de](https://quanta-study.de)

I make products citable by ChatGPT, Perplexity and Gemini - and I ship the system that does it. Most teams have the SEO ideas. I build the production code: programmatic SEO at scale, JSON-LD `@graph`, `llms.txt` / `llms-full.txt`, and RAG citation pipelines.

> I don't consult on GEO. I build the system that makes you citable.

---

## Proof - [quanta-study.de](https://quanta-study.de)

Designed and built solo as Lead Architect (~4 months to production): an AI-native STEM learning platform - B2C SaaS + multi-tenant B2B school system.

`~1,300 commits` · `72 REST routes` · `38+ Firestore collections` · `150+ programmatic SEO/GEO pages` · `45 security-audit passes` · production Next.js 15 + Firebase + Stripe + Gemini/RAG

### The GEO / AI-search stack I built into it

- **`llms.txt` + `llms-full.txt`** - 51 self-contained, citable RAG blocks + 240+ query→answer mappings
- **JSON-LD `@graph` with stable `@id`** - linked Organization / Person / Product / FAQPage / Breadcrumb entities, **server-rendered** (not client-only)
- **RAG citation pipeline** - Semantic Scholar retrieval + CrossRef **DOI verification**, grounded generation, server-side filtering of ungrounded output
- **E-E-A-T & provenance** - author identity, source protocols, verifiable citations per generated unit
- **Answer capsules + FAQ schema** - short, extractable answers built for generative engines
- **Programmatic SEO at scale** - 150+ pages, **IndexNow**, sitemaps, RSS, canonical + meta titles/descriptions, OG images
- **Verified [Wikidata entity Q139500481](https://www.wikidata.org/wiki/Q139500481)** · legal entity AM Creative Tech UG (HRB 47813, Amtsgericht Dresden)

*The Quanta product code stays private - the proof is the live product. The reusable engines behind it are open source (below).*

---

## Open source

Production-grade, zero-dependency TypeScript primitives - most extracted and generalized from Quanta's production codebase. All MIT.

**AI / LLM infrastructure**
- **[resilient-llm-stream](https://github.com/ammmcreativetech-dot/resilient-llm-stream)** - resilience for streaming LLM calls: timeout + backoff retry, SSE keepalive + inactivity watchdog, and a string-literal-aware streaming JSON extractor.
- **[llm-json-repair](https://github.com/ammmcreativetech-dot/llm-json-repair)** - extract complete JSON objects from partial, streaming or malformed LLM output. String-literal-aware brace scanner, LaTeX-safe, field-level recovery, zero dependencies. Built for live Gemini/OpenAI/Anthropic token streams.

**Web platform & correctness**
- **[pwa-background-sync](https://github.com/ammmcreativetech-dot/pwa-background-sync)** - dependency-free helpers for the Background Sync & Periodic Background Sync APIs, with Service Worker messaging and graceful no-ops where unsupported.
- **[unbiased-random-string](https://github.com/ammmcreativetech-dot/unbiased-random-string)** - cryptographically secure random strings via rejection sampling (no modulo bias). Isomorphic browser / Node / edge.

---

## Stack

`TypeScript` · `JavaScript` · `Next.js 15` (App Router, SSR/SSG/ISR) · `React 19` · `Node.js`
`Firebase / Firestore` · `SQL / SQLite` · `Stripe` · `Tailwind` · `Playwright`
`Gemini 2.5 Flash (Genkit)` · `RAG` · `MCP` · `LLM integration`
`JSON-LD / Schema.org` · `llms.txt` · `Programmatic & Technical SEO` · `GEO` · `three.js / KaTeX / MathLive`

---

## Work with me

- 100% remote · 20-30h/week · available now
- 🌐 Live proof: **[quanta-study.de](https://quanta-study.de)**
- 💼 LinkedIn: **[amos-matzke](https://www.linkedin.com/in/amos-matzke-71a73139a/)**
- ✉️ **amos@am-creativetech.com**
