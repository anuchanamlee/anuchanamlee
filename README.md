# Anucha Namlee

**Automation & AI backend engineer** · Thailand (UTC+7) · open to full-time roles and remote contracts

I build backends that run unattended: scheduled workers, LLM pipelines, and chatbots
that small businesses use every day. I care about the boring parts that keep them
alive in production — idempotent jobs, DB-level constraints, tests that prove the
invariant, and logs you can debug from.

📧 anucha.namlee.work@gmail.com

---

## Featured projects

| Project | What it does | Stack |
|---|---|---|
| [**agent-factory**](https://github.com/anuchanamlee/agent-factory) | One spec file in, a deployed Next.js app out. Six headless `claude -p` phases, each gated by a real command (`next build`, migration, `curl`) — a phase passes on exit code, not on the model's word. Resumable from disk. | Bash · Claude Code · Docker |
| [**post-scheduler**](https://github.com/anuchanamlee/post-scheduler) | Scheduled Facebook + Instagram posting for shops: background worker, encrypted page tokens, AI caption drafts in each page's tone, carousel up to 10 images. | Next.js · PostgreSQL · Docker |
| [**typhoon_ocr_api**](https://github.com/anuchanamlee/typhoon_ocr_api) | Thai-language OCR API for images and multi-page PDFs on a self-hosted LLM (Typhoon OCR via Ollama). Bounded parallelism, upload limits, per-page timing. | Python · FastAPI · Ollama |
| [**ai-image-edit**](https://github.com/anuchanamlee/ai-image-edit) | Web app + n8n workflows for Gemini image editing: API-key auth, prompt presets, usage log to Google Sheets. | Next.js · n8n · Gemini |
| [**pdf_JPG**](https://github.com/anuchanamlee/pdf_JPG) | PDF → JPG API built not to fall over: pixel caps per page, disk-spilling ZIP, encrypted-PDF detection. | Python · FastAPI · PyMuPDF |

## Client work (private code — summaries only)

- **LINE booking chatbot for service businesses** — 12 n8n workflows: booking,
  rescheduling, FAQ replies, human handoff, back-office admin. Sold as a template,
  one isolated instance per client.
- **Business website on a VPS** — Next.js + SQLite, migrations safe under concurrent
  start-up, uptime monitoring.
- **License-key service** — issue / validate / move licenses for desktop software
  (Vercel + Supabase), with a customer self-service page.

## Stack

**Backend:** TypeScript, Node.js, Python, FastAPI, Next.js API routes
**Data:** PostgreSQL, SQLite, Supabase, Firebase
**Automation & AI:** n8n, LINE Messaging API, Claude, Gemini, Ollama, OCR
**Ops:** Docker, Linux VPS, Vercel, GitHub Actions

## How I work

- Business rules live in the database (UNIQUE / CHECK / transactions), not only in app code.
- Anything that can be retried is idempotent.
- "Done" means a test or a command proved it — not that it looked fine once.
