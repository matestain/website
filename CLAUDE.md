# CLAUDE.md — website

AI context for the MATESTAIN `website` repository. Read the org-level `.github/CLAUDE.md` first.

---

## Purpose

This repo will become the public landing page for `matestain.com`. It represents MATESTAIN externally — what the company does, who it's for, and how to reach us.

## Current Status

**Not built yet.** This is a placeholder structure. Do not write production code here until development is formally started. If you're here, you're likely setting up the repo or planning.

## Planned Stack

- **Phase 1:** Plain HTML and CSS — static, zero dependencies, deployable to any CDN or static host
- **Phase 2 (if needed):** Next.js — only if dynamic rendering, routing, or API integration becomes necessary

Do not introduce a framework prematurely. Start with the simplest thing that works.

## Placeholder Structure

```
website/
├── index.html        # Main entry point (placeholder)
├── style.css         # Base styles (placeholder)
└── assets/           # Static assets (images, fonts, etc.)
```

This will evolve once development begins. Don't over-engineer the structure before there's real content.

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
