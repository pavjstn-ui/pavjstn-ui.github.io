# FRESH CHAT HANDOVER — pavjust-site

**Date:** 2026-08-13  
**Status:** Portfolio page built and committed  
**Next action:** Add CV download link

---

## What exists

`/Users/macski/Projects/pavjust-site/index.html` — single-file vanilla HTML/CSS portfolio page.

**Design:**
- Dark bg `#0d0d0f`, text `#f0f0ee`, accent `#7b6ff0`
- Sticky top nav: name left, email + GitHub right
- JetBrains Mono + system-ui
- Four sections: About, Projects, Writing, Contact
- Mobile nav toggle (minimal JS)
- `//` prefix on section headers

**Projects included:**
1. OutputGuard — AI safety / EU AI Act / GCP Cloud Run
2. MalVision — ML deployment / YARA / Cloud Run
3. CascadeBench — adversarial ML / benchmark design
4. RefusalGap — LLM evaluation / security tooling
5. agent-loop — Kafka / LLM orchestration / AI infrastructure
6. claude-memory — RAG / ChromaDB / FastAPI / MCP

**Writing section:**
- CascadeBench arXiv preprint (forthcoming)
- OutputGuard Zenodo DOI 10.5281/zenodo.21834704

**Contact:** pjstn@proton.me · github.com/pavjstn-ui

---

## Known gaps

- `PROJECT_PROFILES.md` in pat-vault **does not exist yet** — projects were sourced from session context. Write it before the next site update so the source of truth exists on disk.
- No CV/PDF download link yet — that's the next task.
- GitHub Pages deployment not verified — push was done; check `https://pavjstn-ui.github.io` is live.

---

## Files

| Path | Purpose |
|------|---------|
| `/Users/macski/Projects/pavjust-site/index.html` | Portfolio page |
| `/Users/macski/Projects/pavjust-site/DECISIONS.md` | Design rationale (single-file HTML decision) |
| `/Users/macski/Projects/pat-vault/inbox/raw/20260813_pavjust-site_session-report.md` | Session report |
