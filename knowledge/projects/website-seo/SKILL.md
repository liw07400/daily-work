---
name: website-seo
description: Make and verify PioneerGuard page and SEO changes without overstating indexing, ranking, traffic, or leads.
---
# Website + SEO

## Recorded status
2026-10-28 release record reports a production update at `https://pioneerguardfilm.com`. The certificate pages no longer show the withdrawn XUSHIELD trademark image/PDF; the release check reports those assets return 404. The `/paint-protection-film/`, `/colored-ppf/`, and `/car-wrap-film/` topic pages were sampled; full copy is recorded for English, Chinese, Portuguese and Arabic, with English fallback in other locales. Google Search Console accepted resubmission of `https://pioneerguardfilm.com/sitemap.xml` (10,841 URLs). This confirms submission, not indexing; ranking, traffic and leads remain unverified. Evidence filenames in the release record: `DEPLOYMENT-20261028.md`, `LIVE-VERIFICATION.json`, `SEO-BROWSER-AUDIT.json`.

## Workflow
1. Record page URL, audience, language and purpose; confirm canonical page.
2. Capture before-state for title, meta description, H1, canonical, indexability, internal links and visible copy as applicable.
3. Draft the smallest truthful change matching search intent; save in the actual CMS/source.
4. Reopen the page and inspect rendered copy and metadata; log exact fields as before → after.
5. Check indexing separately in search tools. A saved title does not prove indexing, ranking, traffic or leads.
6. Log evidence and gaps; analytics/CRM evidence is required for traffic and lead claims.
7. For parallel work, keep separate source copies; review the actual delivered files, then release in batches and verify each live page after deployment.
## Performance release workflow
1. Capture the tested URL, deployment/build identifier, device profile, Lighthouse version and before/after evidence. Keep runs comparable; if copy or multiple code areas change, describe the result as an observed before/after, not a controlled experiment.
2. Defer below-the-fold video sources until near the viewport; keep a stable poster, preload only critical first-screen media, and lazy-load/decode lower-page images. Preserve play/pause, carousel behavior and reduced-motion preferences.
3. Build into an isolated output directory and read sitemap/robots from that exact build to avoid stale-preview evidence.
4. After release, verify production HTTP/routes, language variants, key interactions, mobile overflow, and media loading. Record remaining regressions such as FCP/TBT or accessibility warnings.
5. Separate a local Lighthouse run from Google PageSpeed results and field Core Web Vitals. Neither a score nor sitemap submission proves indexing, rankings, traffic, leads or delivery.

## Recorded performance evidence — 2026-10-29
The session release record reports the Chinese homepage deployed at https://pioneerguardfilm.com/zh/ (runtime commit 2c4f347). A local Lighthouse mobile snapshot changed from Performance 65 to 74, LCP 14.3s to 5.0s, and total transfer 11,966 KiB to 1,899 KiB. It was one run before and after several concurrent changes, not a controlled A/B or Google remote/field measurement; FCP and TBT did not improve. Source-side evidence filename: PERFORMANCE-20261029.md.
