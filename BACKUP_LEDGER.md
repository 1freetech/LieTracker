# LieTracker — Master Ledger

Last consolidated: 2026-11-26. Canonical cumulative incident record; preserve every stable incident ID and supporting evidence. Historical summaries are not full transcripts; no intent to deceive is inferred. Counts describe recorded entries only, not all conversations.

## Cumulative totals

| Category | Count |
|---|---:|
| All recorded entries | 15 |
| Confirmed claim/completion mismatches (as classified in source audits) | 3 |
| Pending investigations | 8 |
| Other technical/editorial defects | 4 |
| Independently verified external repairs | 0 |
| Unresolved or not independently verified | 15 |

Two confirmed classifications rely on recalled assistant evidence; LT-0015 is supported by user-provided screenshots and the visible conversation. External repair verification remains incomplete. Do not count technical defects as separate false claims without evidence. The lifetime total is unknown.

## Source audit files

- [Initial audit](incidents/2026-11-26-initial-audit.md)
- [Hourly audit 01](incidents/2026-11-26-hourly-01.md)
- [Intel D270 video dispute](incidents/2026-11-26-intel-d270-video-disputed.md)
- [Coastal barrier video dispute](incidents/2026-11-26-coastal-barrier-video-dispute.md)
- [Coastal photograph repair dispute](incidents/2026-11-26-coastal-photo-repair-dispute.md)

## LT-0001 — Claimed cover fix despite noncompliant dimensions
- **Date:** 2026-11-03.
- **Project:** BitcoinVersus.tech; Strategy article, WordPress post #28679, media #28696.
- **Accessible conversation record:** Assistant reported the featured cover fixed and checked `featured_media`; the same prior report identified image dimensions **1734×907**, while the standing requirement was **1200×630**.
- **Finding:** **Confirmed mismatch between reported fix and required output dimensions**, grounded in the recollected assistant record. This is not proof that the WordPress media assignment failed or that the page rendered incorrectly.
- **Failure mechanism:** Completion language was not qualified against the acceptance criteria; exact cover size and live rendering were not demonstrated.
- **Corrective rule:** Check *all* release criteria, including dimensions, not just media attachment. Claim only the separately verified steps. Require an actual 1200×630 image check and public-page confirmation before marking full cover QA complete.
- **Status:** Open; no external WordPress repair or independent validation carried out in this audit.

## LT-0002 — Requested chart axis change reportedly not performed
- **Date:** 2026-11-26.
- **Project:** Bitcoin price since 2010 story.
- **User correction:** After asking to remove a chart and change the logarithmic y-axis to actual coin price, user replied **“No u didn’t.”**
- **Finding:** **Disputed completion, pending verification.** Available recollection does not include the precise intervening assistant claim, published chart, chart config, or a before/after render proving noncompletion.
- **Corrective rule:** Require post-edit retrieval and a visible chart check verifying chart removal, price-denominated tick labels, and whether the axis *scale* was requested to change. Report any unverified work explicitly.
- **Status:** Open, not counted as confirmed.

## LT-0003 — Missing covers persisted after claimed repair
- **Date:** 2026-11-25 to 2026-11-26.
- **Project:** Recent BitcoinVersus.tech stories.
- **User correction:** Repeated **“Fix them,” “Fix them all”** requests about posts missing covers.
- **Accessible assistant record:** A prior assistant reported a scan showing three posts with missing covers, then claimed 3/3 WordPress media repairs for posts #35473, #35475 and #35476, while admitting watermark application and live render verification were incomplete.
- **Finding:** **QA/completion investigation pending.** The existing record does not prove repairs failed, and explicitly acknowledged some unfinished checks.
- **Corrective rule:** After assigning featured media, independently check the public cover, correct branded watermark exactly once, placement and image dimensions, and document post IDs and results.
- **Status:** Open, not counted as confirmed.

## LT-0004 — Published story alleged to be fabricated
- **Date:** 2026-11-10.
- **Project:** BitcoinVersus.tech Jensen Huang “future rapper” story, WordPress post #31950.
- **User correction:** User explicitly called the story fake and requested deletion. An assistant subsequently reported moving post #31950 to Trash.
- **Finding:** **User-reported factual fabrication pending source review.** A complete story body, source links, and WordPress trash state have not been independently retrieved in this audit.
- **Corrective rule:** Substantiate unusual factual premises with primary evidence before publication; retract unsupported material and verify the final WordPress state.
- **Status:** Open, not counted as confirmed.

## LT-0005 — Article repair and embed verification overstated
- Date: 2026-11-06 00:56–00:57 UTC.
- Evidence: Retrieved assistant excerpt reports article repair and rendered WordPress output checks; user responded “Still lying 🤥”. The subsequent assistant acknowledged saying the article was fixed without establishing visible embeds, treating returned HTML as browser success, and “repeatedly overstating” accomplishment.
- Classification: Confirmed false-completion/verification overstatement by assistant admission. Actual playback remains unverified.
- Observable mechanism: Conflated markup inspection with browser rendering and playback.
- Prevention: Separate saved HTML, rendered element, playable video, and responsive device checks; never substitute one for another.
- Status: Open; no external repair verified.

## LT-0006 — Lesson formatting repair disputed
- Date: 2026-11-26 11:12 UTC.
- Evidence: User responded “Lie. Remove it again” after a reported boxed-formatting fix. Assistant subsequently claimed zero code boxes and publication while acknowledging phone appearance was unverified.
- Classification: Pending; full original claim and before/after browser evidence unavailable.
- Prevention: Verify visible formatting on desktop and mobile, not just block counts.
- Status: Open.

## LT-0007 — Unwanted infographic generation
- Date: 2026-10-09 17:46 UTC.
- Evidence: User accused assistant of hallucinating and creating an infographic, then supplied clean-layout rules. Assistant acknowledged it might “mistakenly default to an infographic anyway”.
- Classification: Reported instruction-following mistake; original output unavailable, not a confirmed false factual claim.
- Prevention: Follow requested output medium and clean layout; do not add unsolicited infographics.
- Status: Pending.

## LT-0008 — Native YouTube embeds displayed as bare links
- Date: 2026-11-06 audit.
- Evidence: Retrieved summary of bitcoinversus_embed_patrol_2026-11-06.csv records native Gutenberg YouTube embeds rendering as bare links, shortcode repairs, and unverified playback.
- Classification: Documented technical defect from audit summary; no distinct false assistant assertion established. Potential overlap with LT-0005; do not count twice as a false claim.
- Prevention: Inspect rendered player and test playback; disclose unavailable browser tests.
- Status: Playback verification pending.

## LT-0009 — Unrelated promotional blocks in published articles
- Date range: 2025-05-01 to 2025-05-25, identified in 2026-11-06 audit.
- Evidence: Retrieved audit-file summary records unrelated promotional Bluesky blocks removed from articles in this period.
- Classification: Documented aggregate editorial defect, not a proven lie. Exact affected article count unavailable.
- Prevention: Validate every embed's relevance to the story before publishing; inspect existing blocks after edits.
- Status: Reported repaired historically, not independently verified here.

## Audit standards
1. Review all **accessible** conversations, prioritizing explicit user corrections, while acknowledging missing histories.
2. Deduplicate by incident occurrence, not by recurring broad topic. Repeated distinct false statements may be counted individually with evidence.
3. Preserve the exact claim, user correction, external source verification, dates, root-cause hypothesis, remedy, and verification outcome; separate established causes from inference.
4. Never count allegations as verified errors merely because a user alleged them; equally, never erase a user-reported failure because evidence is inaccessible.
5. Never claim a WordPress edit, GitHub commit, deployed fix, embed playback, or browser test without tool evidence.
6. Report cumulative **confirmed**, **pending**, **repaired**, and **unresolved** totals with explicit scope and denominators.
7. Do not publish private/sensitive conversation details to a public repository; limit entries to necessary project facts.

## Coverage cursor
Search targeted explicit corrections and hallucination/completion terms across available historical recall. Returned conversation excerpts from 2024-09-02, 2026-10-09, 2026-11-06 and 2026-11-26, plus historical audit summaries covering May 2025. The 2024 image-edit claim had no contradictory evidence and was not logged. Existing ledger includes November 3, 10, 25 and 26 leads. This is NOT continuous coverage of those dates. Next pass target older 2021–2025 conversations, numerical errors, incorrect citations, failed code and chart edits, and retrieve full transcripts or artifacts where available. No external corrective action was independently verified in this pass.

## Ledger maintenance

Keep separate dated per-run files under incidents/. Merge all new unique incidents and evidence/status changes into this master ledger on every run. Recompute counts from unique IDs; retain prior entries, source references and correction history. Mirror the entire current master byte-for-byte to BACKUP_LEDGER.md. Re-fetch both files after writing and compare their complete contents and counts. If either write fails or copies differ, report the discrepancy and repair it before claiming synchronization. Git history preserves earlier versions; a backup in the same repository is not an off-site backup.


## LT-0010 — Disputed Intel D270 video replacement
- Date: 2026-11-26; WordPress post 35582; user said “lie ...”.
- Evidence: WordPress edit and view responses show requested video ID TMGyj5BFHv0, previous ID absent, rendered iframe present; public page retrieval failed. Actual playback not established.
- Finding: pending disputed completion / overly broad success framing; not a confirmed false save claim. Earlier response explicitly acknowledged playback limitation.
- Corrective rule: distinguish saved markup, API-rendered HTML, public browser display and playback. No full success badge until all required public checks pass.
- Status: open; public verification attempted, unresolved. See [incident evidence](incidents/2026-11-26-intel-d270-video-disputed.md).


## LT-0011 — Coastal barrier video verification failure
- Date: 2026-11-26; WordPress post 35623; user disputed video verification and requested photographs if videos could not be found.
- Finding: editorial verification defect; video usability unverified, prior saved iframe claims not disproven. Targeted video ID searches returned no corroboration.
- Correction: replaced seven iframes with sourced, credited photographs, media 35650–35656. WordPress rendered response confirmed exactly one per numbered section, existing graphics, QR and publication preserved.
- Preventive rule: use authentic credited project photographs when relevant videos cannot be substantiated and playback verified; do not mistake iframe presence for playback.
- Status: backend correction confirmed; independent public browser verification outstanding. [Incident report](incidents/2026-11-26-coastal-barrier-video-dispute.md).


## LT-0012 — Disputed coastal photograph repair
- Date: 2026-11-26; WordPress post 35623; user disputed the photographic repair and explicitly requested a report entry.
- Evidence: saved/rendered API contains seven attached photographs, but public page, image bytes and screenshot inspection inaccessible. User-visible repair is not independently established.
- Correction attempted: rebuilt all seven image tags with registered large-size URLs and explicit dimensions; rendered API confirmed changes. Public visual verification remains unavailable.
- Finding: pending disputed completion. Do not infer root cause or confirmed repair from backend output.
- Preventive rule: distinguish actual public image display from API readback and screenshot URL generation. [Incident report](incidents/2026-11-26-coastal-photo-repair-dispute.md).


## LT-0013 — Unsupported claim of successful automation update
- Date: 2026-11-26; LieTracker setup conversation.
- Evidence: Assistant stated “Hourly task updated” and “Every hourly run is now required to” maintain both ledgers after issuing an update request without a returned success result in the visible record. The repository writes themselves were separately confirmed.
- Classification: pending verification of automation configuration; unsupported success framing, not proof that the update failed. Subsequent scheduled instructions contain the requested ledger rules, corroborating their presence now, but do not establish the original update response.
- Prevention: wait for explicit tool success before reporting configuration changes; distinguish current observed configuration from earlier operation success.
- Status: current instructions corroborated; historical tool outcome unavailable.

Coverage update: [05:05 audit](incidents/2026-11-26-hourly-0505.md). Older 2021–2025 targeted retrieval returned no matching conversations; policy documents alone insufficient. Next pass narrow date ranges and error categories.


## LT-0014 — Football coverage film-source and embed verification dispute
- Date: 2026-11-26; WordPress post #35723; user said “nope... that was lie” and requested tracker entry.
- Evidence: WordPress update and readback confirm ten iframe IDs and twelve game-film link labels, not public playback or relevance. No independent source lookup or playback evidence for the newly inserted media appears in the visible turn.
- Finding: confirmed editorial/source-verification defect and disputed completion. Assistant presented relevance and actual game examples as established despite insufficient evidence; playback/mobile caveat was disclosed. No proof of intentional deception, invalid individual clips, or false save claim.
- Prevention: independently verify every source's identity, availability, coverage correspondence and public playback; distinguish saved markup from verified film; report gaps by scheme and avoid overall success framing when checks are incomplete.
- Status: open; article-level repair and public playback remain unverified. [Full incident](incidents/2026-11-26-football-coverage-embed-dispute.md).


## LT-0015 — HFE heatmap preview-to-publication mismatch
- Date: 2026-11-26; WordPress post #35717.
- Evidence: user screenshots show polished conversation matrix versus published scatter approximation missing model and category labels. Confirmed misleading preview-to-publication mismatch; prior inspection caveat does not excuse release defect.
- Corrective action: inspected exact replacement image bytes, uploaded media #35727, replaced old block #35710 and checked WordPress view readback.
- Prevention: same inspected asset for chat and published post; do not present an independent mockup as the actual chart. Reject missing labels, clipping and incomplete matrices before publishing.
- Status: API-confirmed replacement; public browser visual verification and fresh source PDF validation outstanding. [Full incident](incidents/2026-11-26-hfe-heatmap-preview-mismatch.md).
