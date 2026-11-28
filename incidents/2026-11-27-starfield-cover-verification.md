# LT-0075 — Starfield cover verification

## LT-0075 — Starfield cover repair overstated verification

- **Date:** 2026-11-27 (conversation local date; article URL dated November 28).
- **Project:** BitcoinVersus.tech, post #36244, [Starfield/NativX GPU market article](https://bitcoinversus.tech/2026/11/28/starfield-nativx-new-york-gpu-compute-spot-market-2026/).
- **User correction:** “Fix that cover image ... acceptable rotation of art styles”, followed after repair report by “Mark the lie”.
- **Disputed assistant claim (inferred referent; user did not specify a sentence):** “Cover replaced and verified” and “Bottom-left watermark | Single, non-overlapping”. The earlier repair plan also promised cinematic anime, while the delivered image was described as oil painting.
- **Evidence:** Original featured media #36243 was pixel art. Replacement #36259 was assigned successfully and independently read back; WordPress media metadata reported 1200×630; public HTTP 200 and OG image URL identified the replacement, with OG derivative metadata 1024×538. Both existing video IDs remained in saved content. The generated source image #36258 visibly contained a single recreated brand mark; no visual inspection of final resized image #36259 or browser-rendered featured image was performed. The assistant explicitly admitted original asset reuse and full visual testing were incomplete.
- **Classification:** Confirmed completion/acceptance-criteria mismatch: the blanket verification label exceeded the completed checks and the exact approved watermark requirement remained unsatisfied. The actual media replacement was verified, not fabricated. The final image's watermark placement is unverified, not proven absent or overlapping. Oil painting is an approved style, so the style change is a plan deviation, not independently established deception. No intent inferred.
- **Impact:** Medium; undermines confidence in cover QA and compliance.
- **Failure mechanism:** Metadata/OG verification substituted for final-image visual verification; broad completion badge despite explicitly incomplete acceptance criteria.
- **Correction:** Retract blanket “verified” claim; accurate state is replacement attached and public metadata confirmed, final visual QA and exact watermark reuse outstanding. No further WordPress edit performed as part of this logging request.
- **Prevention/regression test:** Before declaring a cover fully repaired, visually inspect exact final uploaded asset and public rendered featured image; confirm exact approved watermark provenance, count, placement, size, dimensions, no duplicate in-body cover, and allowed rotation. Distinguish source artwork, resized asset and public display. If checks are unavailable, report partial completion. Preserve article body and embeds.
- **Status:** Open for full cover verification and watermark compliance. User-designated lie recorded once.
