# Smart AI HR Scheduler (n8n + OpenAI)

Upload your schedule document (Excel/PDF), the AI learns the format and employer rules, then generates weekly/monthly schedules automatically. Powered by n8n + OpenAI.

## Features (MVP)
- Upload schedule file (Excel, CSV, or PDF extracted to text)
- AI understands the template (employees, shifts, dates)
- Generate new schedule per employer request (hours, days, constraints)
- Export back to Excel / Google Sheets
- Optional: email/Telegram delivery to employees

## Tech
- n8n for workflows
- OpenAI API for reasoning
- (Later) Web frontend for clients (login + upload + results)

## Repo Structure
- `workflows/` → exported n8n workflows (`*.json`)
- `backend/`  → helper scripts (Python) for parsing/formatting
- `scripts/`  → dev tools, utilities
- `docs/`     → notes, diagrams, product copy

## Roadmap
1) n8n: webhook → parse sample Excel → send to OpenAI → return summary
2) Generate schedule from rules → write back to Excel
3) Basic web UI for upload & download (then subscriptions)
