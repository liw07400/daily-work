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
7. Read the current workspace collaboration rules first. If the user has selected a shared checkout, coordinate one writer per overlapping file, preserve unrelated changes and use the agreed preview; use separate copies when required by the current workflow. Review delivered files before releasing and verify live pages separately.
## Performance release workflow
1. Capture the tested URL, deployment/build identifier, device profile, Lighthouse version and before/after evidence. Keep runs comparable; if copy or multiple code areas change, describe the result as an observed before/after, not a controlled experiment.
2. Defer below-the-fold video sources until near the viewport; keep a stable poster, preload only critical first-screen media, and lazy-load/decode lower-page images. Preserve play/pause, carousel behavior and reduced-motion preferences.
3. Build into an isolated output directory and read sitemap/robots from that exact build to avoid stale-preview evidence.
4. After release, verify production HTTP/routes, language variants, key interactions, mobile overflow, and media loading. Record remaining regressions such as FCP/TBT or accessibility warnings.
5. Separate a local Lighthouse run from Google PageSpeed results and field Core Web Vitals. Neither a score nor sitemap submission proves indexing, rankings, traffic, leads or delivery.

## Recorded performance evidence — 2026-10-29
The session release record reports the Chinese homepage deployed at https://pioneerguardfilm.com/zh/ (runtime commit 2c4f347). A local Lighthouse mobile snapshot changed from Performance 65 to 74, LCP 14.3s to 5.0s, and total transfer 11,966 KiB to 1,899 KiB. It was one run before and after several concurrent changes, not a controlled A/B or Google remote/field measurement; FCP and TBT did not improve. Source-side evidence filename: PERFORMANCE-20261029.md.

## Shared preview and interface checks — 2026-10-30
- The recorded PioneerGuard decision uses the existing preview on port 3184 and one shared checkout. Recheck workspace AGENTS.md and .collab/STATE.md before edits; preserve valid language paths, query filters and anchors. Do not deliver an old preview from another port.
- Reuse the running development service. If a build is needed, set a distinct NEXT_DIST_DIR; do not build into the active service output or restart services simply to coordinate links.
- For galleries, keep a stable frame and avoid scrollIntoView on ordinary image changes. Verify hover, keyboard, modal focus return/Escape, scroll locking, reduced motion, mobile layout and URL/scroll stability. Distinguish actual touch testing from code inspection.
- For added feedback details, verify the source-to-detail mapping, return links, each locale route, metadata and invalid-ID 404 behavior. Keep source screenshots private and sanitized.
- Date checks to the exact version tested. A prior build audit does not validate later media/layout changes; a local route or sitemap is not a public release or indexing result.

## Sitewide motion and media audit
1. Inventory the source assets and rendered routes. Use contact sheets to triage large image sets; use OCR to find possible text or marks, then visually inspect candidates and final displayed assets because OCR can miss small details.
2. Preserve original product assets and factual specifications. Apply approved display replacements through a scoped presentation mapping where possible. Use genuine, model-relevant vehicle photos; keep supplier/material facts separate from competitor branding and unrelated logo showcases.
3. Verify motion and image behavior at desktop, embedded-preview and mobile widths, with reduced motion enabled. Check filter/pagination insertions, hover or keyboard transitions, URL/scroll stability, and images filling their frames.
4. Record the exact route count, viewport sizes, image and console checks, and whether checks were final or earlier broad sampling. A local preview is not a production release.

## Navigation, grouped content and Chinese fonts
- For a menu that closes as the pointer moves from its trigger, inspect the gap and shared hover region. Verify crossing into the menu and activating a destination separately. Counting anchors and receiving HTTP 200 do not prove a card can actually be clicked; record keyboard activation separately where tested. Preserve locale paths and product filters.
- When grouping existing content, inventory the original items before rearranging them, then check category jumps, arrows and scroll transitions against that inventory. Include a short embedded-preview height as well as desktop/mobile widths; a height threshold can silently disable the interaction.
- For self-hosted Chinese font subsets, preserve the font licence and compare the final rendered copy's characters with the font cmap. Repeat after copy changes, and inspect the loaded font and supported weight range in the browser. A successful subset check covers only the tested text.

## Video sections and third-party visual references
- When a supplied clip must start at a specified source time, preserve the original and verify the rendered clip's duration and first frame. Test viewport sizing, load deferral, offscreen/background pause, loop and manual controls, reduced motion, mobile controls, route/anchor behavior and every locale where the component is reused.
- Label competitor photos as reference material, link the source page and keep them distinct from PioneerGuard product photos. A reachable image URL does not establish usage rights; confirm permission or replace the image before public release. Recheck a preview after later edits and report only the version actually tested.

## Product details and certificate presentation
- Verify desktop sticky galleries within their product section and below navigation, then check that mobile galleries return to normal flow. Test thumbnail/lightbox selection, lower-to-upper size synchronization and inquiry contents on representative models. Audit generated detail coverage separately from source-data gaps; a successful all-record marker check is not all-record browser interaction testing.
- For certificate walls, preserve links to originals and identify each document's legal holder and actual brand. A document shown under About does not automatically certify the website brand. Record local reintroductions separately from earlier production removals, and do not infer current legal validity from a readable PDF. Check final requested removals of counts/copy and the original viewer independently of earlier layout prototypes.

## Preview switching and playback checks
- For a built preview, check listener ownership, expected build identity and rollback target before switching under the current authorization. Test HTTP readiness separately from hydrated browser state: query-driven content created after client rendering may be absent from initial HTML. Wait for the rendered collection, decode images and check all model selections before deciding that the new build failed. After any fallback, recheck which build is actually served. Do not bypass an execution-policy rejection through another startup mechanism.
- Test animation thresholds in a short desktop window as well as standard desktop/mobile. For autoplay, verify manual navigation, pause/resume, skip target and button alignment; pause when offscreen, hidden or covered by a media modal, and preserve visible static content under reduced motion. Check hero framing on narrow screens, anchor behavior and whether its original image duplicates product allocations. Keep each QA report tied to its tested version; an earlier broad pass does not prove every later edit passed the same checks.
- Apply the latest requested control design: the 2026-11-06 local homepage revision removed decorative play/pause toggles and the feedback counter while retaining viewport-based autoplay, manual navigation and reduced-motion handling. Earlier button-presence checks describe the previous version. Verify the current control set, native controls in opened media viewers, focus/interaction behavior and hover motion separately; a successful animation test is not a complete accessibility audit.
- When a model query reuses a detail route, check that the chosen model drives title, parameters, gallery and inquiry variant together. Preserve the general catalogue and unresolved legacy SKU links. A new query-driven model card is not automatically a new static page or an indexed URL. After gallery layout changes, test desktop sticky bounds, short-screen control visibility, mobile normal flow and retained anchors/disclaimers.
