# Job Co-Pilot — interactive prototype

An agentic job-search co-pilot built for an international student in Sydney. It:

1. **Discovers** IT roles (real builds use the free [Adzuna API](https://developer.adzuna.com/); Seek/LinkedIn are pasted in, never scraped).
2. **Dual-track ranks** them — a **PR-builder** track (onshore AU, study-aligned, builds PR-qualifying experience) and a **freedom/income** track (fully remote, flagged as 0 PR value).
3. **Tailors a résumé** per role — honesty-locked, never fabricates.
4. **Runs the toughest recruiter** — an adversarial reviewer scores the résumé (ATS match + 1–10) in a generator↔critic loop until it passes, or emits a **gap report** roadmap instead of a fake résumé.
5. **You approve** → a ready-to-submit **packet** is assembled. You click submit (no bots, no ToS risk).

This page is a **self-contained front-end prototype** — the recruiter gauntlet runs as a client-side simulation over sample roles, no live API calls or personal data.

## Run locally

Just open `index.html`, or:

```bash
npx serve .
```

## Verified facts behind the design

- Student visa (subclass 500): **48 hrs/fortnight** during study sessions. ([Study Australia](https://www.studyaustralia.gov.au/en/plan-your-move/your-guide-to-visas/student-visa-subclass-500))
- PR points require **physically-in-Australia** work — remote-from-abroad builds no PR-qualifying experience. ([Agape Henry Crux](https://www.ahclawyers.com/news-articles/25/11/12/claim-work-experience-points-for-gsm-onshore-vs-offshore-remote-work))

> Not migration advice. Verify any PR/visa specifics with a MARA-registered agent.

Built with [Claude Code](https://claude.com/claude-code).
