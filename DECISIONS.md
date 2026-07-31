# Design Decisions

## Single-file static HTML over a framework

**Date:** 2026-07-31  
**Context:** Personal CV/portfolio for Pavol Just, deploy target GitHub Pages.

**Decision:** One `index.html`, inline `<style>`, no JS, no build step, no dependencies.

**Why:**

A CV site has one job: communicate who you are in under 30 seconds. Every layer of tooling added to accomplish that job is a liability — build failures, dependency rot, hydration flicker, bundle bloat. A single HTML file:

- Deploys in one `git push` — no CI, no Actions, no npm install
- Loads instantly from GitHub Pages CDN with zero JS parse overhead
- Has zero attack surface beyond the HTML spec itself (relevant for an AI security researcher's own site)
- Will render correctly in 10 years without a single `npm audit fix`
- Can be inspected, forked, or handed to anyone by opening one file

The Karpathy precedent (karpathy.github.io) validates this: a minimal, fast, text-first personal page signals taste and confidence more than a Next.js portfolio ever could.

**Tradeoff acknowledged:** Adding a blog or dynamic content later would require either a static site generator (Hugo, Eleventy) or a separate service. Acceptable — cross that bridge if and when needed. Current scope is a CV, not a blog.
