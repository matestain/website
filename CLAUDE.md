# CLAUDE.md — website

AI context for the MATESTAIN `website` repository. Read the org-level `.github/CLAUDE.md` first.

---

## Purpose

This repo will become the public landing page for `matestain.com`. It represents MATESTAIN externally — what the company does, who it's for, and how to reach us.

## Current Status

**Live landing page** at https://matestain.com — minimal HTML/CSS, visual style aligned with the brand guide. Functional email drop. Website v1 (full site) is still pending development.

### Live infrastructure

- **Hosting:** Cloudflare Pages, Git-connected to `main` branch, auto-deploy on push
- **Email drop:** Cloudflare Function at `/api/subscribe` → Resend API
  - Audience: `matestain`, Segment: `General`
  - Env vars required in Cloudflare Pages: `RESEND_API_KEY`, `RESEND_AUDIENCE_ID`

### Website v1 — Planned Stack

- **Phase 1:** Plain HTML and CSS — static, zero dependencies
- **Phase 2 (if needed):** Next.js — only if dynamic rendering, routing, or API integration becomes necessary

Do not introduce a framework prematurely. Start with the simplest thing that works.

## Current Structure

```
website/
├── index.html        # Landing page
├── style.css         # Base styles
└── assets/           # Static assets (images, fonts, etc.)
```

## Design Direction

- Tone: confident, technical, Argentine — not corporate-generic
- Typography and color: derive from the `brand` repo
- Mobile-first layout

## What Not to Do

- Do not add JavaScript frameworks, build tools, or npm dependencies until the stack decision is made
- Do not deploy to production without Lucas's explicit sign-off
- Do not use placeholder text (Lorem Ipsum) — leave sections blank or clearly marked `[TODO]`

## Commit Conventions

Follow org-level Conventional Commits. Scope: `website`.
```
feat(website): add hero section
fix(website): correct mobile nav overflow
chore(website): add base HTML structure
```

---

_Part of the MATESTAIN organization — see `.github/CLAUDE.md` for org-wide context._
