---
name: openclaw-seo-content-writer
description: Create, QA, publish, deploy, and index SEO blog content in an OpenClaw workflow using a Tony + Peter lane split. Use when the task is to write or ship SEO blog posts, run safe-template blog production, perform publish readiness QA, deploy blog updates, verify live visibility, submit URLs to Google Search Console, or operate a repeatable SEO content pipeline for OpenClaw/ClawLite-style sites.
---

# OpenClaw SEO Content Writer

Use this skill to run a full SEO blog production lane instead of treating “write a blog post” as only a drafting task.

## Core model

Split ownership clearly:

- **Tony** owns draft generation, safe-template normalization, preflight, content-quality gating, source publish readiness, and artifact receipts.
- **Peter** owns deployment, live verification, indexability checks, Google Search Console submission, and indexing-status receipts.

Never collapse these into one fuzzy “content done” state.

## Required workflow

1. **Gather same-day inputs**
   - keyword / topic target
   - audience + search intent
   - Hunter research / evidence / proof links
   - brand positioning + CTA source
2. **Write the draft batch**
   - Use a stable SEO skeleton, not freeform prose.
   - Ensure every draft answers the query directly and has enough structure to survive QA.
3. **Normalize through safe template**
   - Stamp template metadata.
   - Ensure every draft contains a quick answer, TL;DR, scannable sections, FAQ, conclusion, CTA, and source/proof notes.
4. **Run publish gates**
   - structural preflight
   - content-quality audit
5. **If not publishable, recover correctly**
   - Do not pad with filler.
   - Call Hunter for bounded same-day recovery research first.
   - Only downgrade or replace the topic if Hunter also cannot make it longform-worthy.
6. **Source publish**
   - Only after preflight + quality audit pass.
   - Write a structured source-publish receipt.
7. **Peter closeout**
   - deploy production
   - verify live URL and `/blog`
   - verify canonical / sitemap / noindex / discovery
   - write deployment + indexability receipts
8. **Search Console follow-through**
   - submit only `INDEX_READY` URLs
   - write GSC submission receipt
   - check indexing status later and write GSC status receipt

## Non-negotiable rules

- **No filler padding.** If word count is thin, add real information or trigger research recovery.
- **No publish without receipts.** Preflight, quality audit, source publish, deploy, and indexability should all leave artifacts.
- **No “live” claims without Peter verification.** Code-ready is not live.
- **No GSC submission before indexability passes.** Live + self-canonical + sitemap + `/blog` discovery must be true first.

## Minimum draft contract

Every publish candidate should have:

- direct answer / quick answer
- TL;DR
- 4+ substantial H2 sections
- comparison table or clear scannable structure
- FAQ with at least 4 real questions
- conclusion
- CTA
- source / proof notes
- enough specificity, proof, and search-intent coverage to be publishable

## Recovery logic

If a draft batch fails because it is thin, weakly evidenced, or not publishable:

1. classify the problem
2. call Hunter for more research
3. rewrite once with stronger evidence / FAQ material / angles
4. rerun gates
5. only then downgrade or replace the topic if still too weak

## Receipts to maintain

Use the same style of structured receipts for every lane:

- preflight receipt
- content-quality audit receipt
- source-publish receipt
- deployment receipt
- blog indexability receipt
- GSC submission receipt
- GSC index-status receipt

## References

Read these files when needed:

- `references/tony-pipeline.md` — drafting, gating, recovery, and source publish flow
- `references/peter-closeout.md` — deploy, live verification, indexability, and closure rules
- `references/gsc-indexing.md` — Search Console submission and indexing-status workflow
- `references/receipt-contracts.md` — receipt expectations and truth states
