# Abdelhamid Bali — AI engineer (LLM · RAG · agents · evaluation)

I build LLM products for Arabic- and French-speaking users, and I test them like production software:
retrieval that cites its source, agents that never invent a price, and evaluations that run in CI.

Freelance, remote, based in Algeria.

## Live demos (self-hosted)

| Demo | What it shows |
|---|---|
| [Ask your document](https://abdelhmid-vostro-1015.tailc599d9.ts.net/) | RAG over an uploaded PDF (Arabic included): answers with the page number, refuses when the answer isn't there |
| [Invoice reader](https://abdelhmid-vostro-1015.tailc599d9.ts.net/invoices) | Invoice image/PDF → structured fields → Algerian SCF journal entry, tax-ID checks, Excel / PC Compta export |
| [Auto-parts sales agent](https://abdelhmid-vostro-1015.tailc599d9.ts.net/agent) | WhatsApp-style agent that understands Algerian dialect and French part names, on a fictional catalog |

They run on my home server, so they can occasionally be offline.

## Selected work

- **[llm-eval-suite](https://github.com/abdlamid88-droid/llm-eval-suite)**: how I test the demos above. Unit tests with a mocked LLM, live API tests, Playwright, and promptfoo evals, all in GitHub Actions. Seven defects documented with root cause and fix.
- **[bayyinah-ai](https://github.com/abdlamid88-droid/bayyinah-ai)**: grounded RAG for verifying hadith attribution. Hybrid search (pgvector + lexical), two-gate matching and explicit abstention when no source is found.
- **[edge-gateway-blueprint](https://github.com/abdlamid88-droid/edge-gateway-blueprint)**: IIoT edge gateway with Modbus/KNX ingestion, SQLite WAL buffering, and store-and-forward to MQTT with QoS 1.
- **[payagentic-engine](https://github.com/abdlamid88-droid/payagentic-engine)**: agent-to-agent commerce prototype with PayPal two-phase settlement (authorize → capture).
- **[saudi-invoice-saas](https://github.com/abdlamid88-droid/saudi-invoice-saas)**: ZATCA e-invoicing prototype exposed as an MCP server (TLV QR encoding, SQLite archive).

## Stack

Python · FastAPI · PostgreSQL / pgvector · Gemini and OpenAI-compatible models (Ollama, vLLM) · structured output with Pydantic · Docker · pytest · Playwright · promptfoo · GitHub Actions

---

مهندس ذكاء اصطناعي من الجزائر: أبني تطبيقات LLM وRAG ووكلاء محادثة للعربية والفرنسية، وأختبر جودتها بالاختبارات الآلية والتقييم المستمر.
