# Anucha Namlee

**Backend & Automation Developer** · Computer Science graduate (RMUTI, 2026) · Nakhon Ratchasima, Thailand (UTC+7) · open to full-time roles and remote contracts

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
| [**post-scheduler**](https://github.com/anuchanamlee/post-scheduler) | Scheduled Facebook + Instagram posting for shops: worker that claims jobs with `SKIP LOCKED`, idempotent retries, AES-GCM encrypted tokens, AI captions and images with cost caps. | Next.js · PostgreSQL · Docker |
| [**Buddy-pay**](https://github.com/anuchanamlee/Buddy-pay) | Split a restaurant bill to the satang and get a PromptPay QR per person. Integer money math, CI, unit + E2E tests, [live demo](https://buddy-pay-eta.vercel.app). | Next.js · TypeScript · Firebase |
| [**typhoon_ocr_api**](https://github.com/anuchanamlee/typhoon_ocr_api) | Thai-language OCR API for images and multi-page PDFs on a self-hosted LLM (Typhoon OCR via Ollama). Bounded parallelism, upload limits, per-page timing. | Python · FastAPI · Ollama |
| [**ai-image-generation**](https://github.com/anuchanamlee/ai-image-generation) | Image generation as a service: admin-defined prompt tasks, Gemini via n8n, HMAC-signed admin sessions with tests. | Next.js · Prisma · n8n · Gemini |
| [**license-key-admin-demo**](https://github.com/anuchanamlee/license-key-admin-demo) | Admin panel for software license keys plus a customer self-service machine move. Runs on a built-in mock backend. | Next.js · TypeScript |

More: [gemini-image-edit](https://github.com/anuchanamlee/gemini-image-edit) (n8n + Gemini) ·
[pdf_JPG](https://github.com/anuchanamlee/pdf_JPG) (FastAPI) ·
[n8n-docker](https://github.com/anuchanamlee/n8n-docker) ·
[slipledger](https://github.com/anuchanamlee/slipledger) (Flutter) ·
[live portfolio](https://portfolio-sigma-seven-k509pz4cai.vercel.app)

## Experience

- **Freelance developer, Fastwork** (Jan 2025 – present): web apps, back offices and LINE chatbots for small businesses.
- **Internship Developer, บริษัท สิทธิประชา คอร์ปอเรชั่น จำกัด** (Nov 2024 – Feb 2025, full-time): REST APIs with NestJS (JWT login, email OTP, OCR integration).

## Client work (private code — summaries only)

- **LINE booking chatbot for a home-cleaning shop** — 30+ n8n workflows: booking,
  availability, team assignment, payment slips, AI replies, back-office admin
  (pre-launch; the slip check and AI replies are not yet tested against live services).
  Built as a template, one isolated instance per client. A separate 12-workflow
  starter template is also kept.
- **Business website** — Next.js + SQLite on Hostinger, migrations safe under
  concurrent start-up, uptime monitoring.
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
