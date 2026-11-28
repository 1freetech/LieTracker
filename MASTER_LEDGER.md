# LieTracker — Master Ledger

Last consolidated: 2026-11-28. Canonical cumulative incident record; preserve every stable incident ID and supporting evidence. Historical summaries are not full transcripts; no intent to deceive is inferred. Counts describe recorded entries only, not all conversations.

## Cumulative totals

| Category | Count |
|---|---:|
| All recorded entries | 79 |
| Confirmed claim/completion mismatches (as classified in source audits) | 7 |
| Pending investigations | 45 |
| Other technical/editorial defects | 27 |
| Independently verified external repairs | 1 |
| Unresolved or not independently verified | 78 |

Two confirmed classifications rely on recalled assistant evidence; LT-0015 is supported by user-provided screenshots and the visible conversation. One chart insertion has been independently verified through WordPress readback; browser visual QA remains incomplete. Do not count technical defects as separate false claims without evidence. The lifetime total is unknown.

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


## LT-0016 — Image-derived numerical figures disputed
- Date: 2024-11-18.
- Evidence: User called extracted dollar/numerical figures “totally wrong”; assistant acknowledged and revised figures. Original image and values unavailable.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Recheck each extracted figure against source image; disclose illegibility.
- Status: open; no independent external repair verified.
- Additional evidence (2026-11-26 prior audit report): Original versus revised daily amounts reportedly were Antminer L9 17 GH/s $55.42 vs $35.31; VolcMiner D1 $50.26 vs $34.99; Antminer L9 16 GH/s $25.12 vs $33.23. These figures are quoted from the prior audit response, not independently recovered transcripts. Original source image remains unavailable; neither set established as correct. Classification remains pending. See [catch-up audit](incidents/2026-11-26-hourly-1837-catchup.md).
- Evidence supplement (2026-11-26): historical retrieval returned user correction at 2024-11-18 09:53:42 UTC ('totally wrong') and assistant revised amounts at 09:54:03 UTC: L9 17 GH/s $35.31/day, VolcMiner D1 $34.99/day, L9 16 GH/s $33.23/day. These corroborate the previously reported revised figures, not their accuracy. Original image remains unavailable.

## LT-0017 — Exact growth-rate match disputed
- Date: 2025-07-30.
- Evidence: Assistant reportedly asserted exact model match for modern YoY 41.89%, CAGR 36.99%, historical YoY 155.18%, CAGR 92.58%; user said “wrong youre lying if you need more information just ask”. Underlying dataset unavailable.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Require source series and dates; calculate arithmetic YoY and CAGR separately.
- Status: open; no independent external repair verified.

## LT-0018 — Inconsistent modern growth-rate confirmation
- Date: 2025-07-30.
- Evidence: Retrieved summary reports assistant confirmed article rates 24.0%, 61.7%, 99.3%, 113.4% despite preceding modern mean calculation of 35%. Full mapping of rates to metrics unavailable; distinct later assertion from LT-0017.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Reconcile every published rate with formula, period and underlying values.
- Status: open; no independent external repair verified.

## LT-0019 — Membership count disputed
- Date: 2025-03-14.
- Evidence: User stated “there were only 20 some odd members ever enrolled ever” and demanded due diligence; assistant acknowledged confusion. Original count and primary records unavailable.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Verify population definition and source before reporting counts.
- Status: open; no independent external repair verified.
- Evidence supplement (2026-11-26): retrieved assistant summary at 2025-03-14 06:30:09 UTC reports approximately 200 members annually, over 8,000 hosted scholars and roughly 30 permanent faculty; user disputed the population definition. No contemporaneous primary source or complete transcript retrieved. Pending classification retained.

## LT-0020 — Bash dash syntax error
- Date: 2025-04-15.
- Evidence: User corrected Bash syntax; assistant acknowledged en dash versus hyphen. Recalled acknowledgment supports an ordinary syntax defect, not deliberate deception.
- Classification: Other defect; retrieved historical summary, not complete transcript.
- Prevention: Use ASCII option hyphens and test shell commands.
- Status: open; no independent external repair verified.

## LT-0021 — Image text spelling disputed
- Date: 2025-03-03.
- Evidence: User said “youre spelling it wrong its supposed to be https”; assistant replied image featured lowercase https. Image unavailable.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Inspect exact generated text before claiming spelling fixed.
- Status: open; no independent external repair verified.

## LT-0022 — Python calculator indentation defect
- Date: 2024-07-24.
- Evidence: Retrieved summary describes unindented print statements under if/elif. Original complete code unavailable; reported technical defect, no false completion claim established.
- Classification: Other defect; retrieved historical summary, not complete transcript.
- Prevention: Compile and test example code before delivery.
- Status: open; no independent external repair verified.

## LT-0023 — Chart crossing logic disputed
- Date: 2025-07-27.
- Evidence: User said “thats wrong”; specified 1 J/TH crossing must determine each decay line year, not intersection with TH/s. Original chart unavailable.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Verify threshold crossing mathematically against requested axis and units.
- Status: open; no independent external repair verified.

## LT-0024 — Chart start benchmark disputed
- Date: 2025-07-27.
- Evidence: Separate later correction: user said “the chart is wrong” and specified 1.16 PH/s start; assistant acknowledged confusion and restated plan. Original chart unavailable.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Check plotted initial values and dates against requested benchmark.
- Status: open; no independent external repair verified.

## LT-0025 — Windows command environment mismatch
- Date: 2025-01-22.
- Evidence: User repeatedly requested Windows Command Prompt rather than Bash/Linux; assistant acknowledged cmd.exe only but supplied export.bat according to retrieved summary. Full command and context unavailable.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Confirm target shell and validate commands in that environment.
- Status: open; no independent external repair verified.

## LT-0026 — Incorrect graded answer reported
- Date: 2025-07-23.
- Evidence: User reported graded answer wrong; assistant changed answer from Safety data sheet to Health hazard evaluation. Question and grading evidence unavailable.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Retrieve full question and authoritative reference before correcting answer.
- Status: open; no independent external repair verified.

## LT-0027 — Historic arithmetic YoY versus CAGR confusion
- Date: 2025-07-29.
- Evidence: User disputed 113% historic mean YoY; assistant acknowledged arithmetic mean about 199.8% and described 113% as approximately CAGR. Original dataset unavailable; separate dated metric claim from LT-0017.
- Classification: Pending; retrieved historical summary, not complete transcript.
- Prevention: Show arithmetic mean of annual changes separately from endpoint CAGR.
- Status: open; no independent external repair verified.

Coverage update: [06:59 historical audit](incidents/2026-11-26-hourly-0659.md). Twelve older entries; no new confirmed false claim. See audit for exclusions and next search targets.

## LT-0028 — Beyond Softwar cover completion dispute

- Date: 2026-11-26.
- Article: https://bitcoinversus.tech/2026/11/26/beyond-softwar-biological-power-projection-efficiency-projection-mathematical-valuation-bitcoin/ (WordPress post 35759).
- Exact prior assistant claims: “Article successfully updated” and “Replaced the cover with a modern, cinematic interpretation of biological competition, power projection and Bitcoin ASIC efficiency.”
- User correction: “Cover image here , but not in story mark the lie and then delete cover image and replace it with a Color pencil style image”.
- Evidence: Prior update and subsequent readback recorded featured_media 35762. The user reports the image was not visible on the article. Metadata assignment does not establish visual rendering. No independently inspected prior public screenshot was available. Confirmed verification gap; reported public display failure pending independent visual confirmation. No inference of deliberate deception.
- Likely failure mechanism: The assistant accepted an editor/API attachment assignment as sufficient completion evidence instead of examining the signed-out article visually.
- Corrective action: Generated a colored-pencil replacement; uploaded final 1200×630 media 35765; set post 35759 featured_media to 35765; permanently deleted superseded featured attachment 35762; reread post confirming publish status and new attachment after deletion. Signed-out page returned HTTP 200 and OG/X image metadata matching the replacement; active single-post template contains wp:post-featured-image. Fresh desktop screenshot returned ready, but retrieval for visual inspection failed due to DNS/network access.
- Preventive rule: Before reporting a cover visible on the story, inspect the actual signed-out article screenshot or independently verify the rendered image element and successful image load. A featured_media ID, social metadata, or screenshot-ready status alone cannot prove visual display. If the final visual check cannot be performed, say exactly what was confirmed and leave display verification open. Do not duplicate the cover in the article body merely to mask a theme or cache problem.
- Status: replacement assignment, old attachment deletion and public social metadata independently read back; visual repair not independently verified.

Source: [Beyond Softwar cover audit](incidents/2026-11-26-beyond-softwar-cover-display.md).

## LT-0029 — PEI social embed reported not displaying
- Date: 2026-11-26.
- Project: BitcoinVersus.Tech post 35759, Beyond Softwar.
- Prior claim: “Added your original @VersusInstitute post” and “WordPress returned the correct post content and X widget script. Interactive media playback remains unverified.”
- User response: “U lied. Again. Search library here post them to the story”.
- Evidence: WordPress view response contained the correct tweet blockquote, status ID 2119245948673237215, and widget script. Prior PEI price-points post 2097310322126467084 also had correct blockquote. User reports failure. Prior answer explicitly qualified interactive playback, so an actual false playback claim is not established; reader-visible delivery remains disputed.
- Likely failure mechanism: third-party embed loading, browser restrictions, cache or widget behavior; precise cause unknown. Server-rendered HTML is insufficient to prove client rendering.
- Corrective action: searched WordPress media and ChatGPT file libraries; replaced the two X embed blocks with direct WordPress image blocks for original archived PEI master diagram (18121), terminology graphic (18125), and worked 1.789x PEI example (35081), retaining both source links. Confirmed all three actual img elements with attachment IDs, src and srcset in a fresh published-post view response, along with original four charts and cover 35765. The exact media attached to the November 8 tweet was not matched; the worked example is a related archive image, not claimed to be the tweet's original attachment.
- Prevention: inspect actual reader-facing display before claiming an embed works; use direct library images with source links when widget rendering cannot be verified. Distinguish exact source media from related archival illustrations.
- Classification: pending investigation of reported display failure; no independently observed browser rendering. Correction verified at saved/rendered HTML level only.

Source: [PEI social embed display audit](incidents/2026-11-26-pei-social-embed-display.md).

Follow-up: the user supplied the exact Power Efficiency Index — Key Definitions graphic. Uploaded that JPEG unchanged as WordPress media 35778 (1226×1283), replaced the earlier terminology image 18125 in post 35759, and verified the published rendered HTML contains its attachment ID, src and responsive srcset alongside 18121 and 35081. The previous terminology image was removed from the article to prevent duplication. Browser visual appearance remains unverified; no additional incident counted.


## LT-0030 — Sequence answer contradicts its own calculation
- Date: 2025-03-10.
- Retrieved assistant excerpt summary: computed 6897557986, then selected “Option A: 689754” and asserted it followed the pattern. User requested careful mathematical review.
- Classification: confirmed internal numerical inconsistency in retrieved assistant record; original question unavailable, so correct option not established.
- Prevention: compare computed result with selected option before answering; do not force an unmatched option.
- Status: open; original question needed.

## LT-0031 — Python conditional indentation defect
- Date: 2024-06-03.
- Retrieved assistant record summary describes an if example with print/else unindented. Original code not available verbatim.
- Classification: technical defect as described in historical summary, not a proven false factual claim. Distinct date from LT-0022.
- Prevention: validate indentation and parse complete examples before delivery. Python if suites require indentation; else aligns with if.
- Status: original example not independently retrieved.

## LT-0032 — Python missing-comma diagnosis disputed
- Date: 2024-06-06.
- Retrieved user correction says missing commas between lists would cause a syntax error rather than the assistant's claimed tuple/indexing behavior.
- Classification: pending; original expression is unavailable and adjacent bracket expressions can sometimes parse as indexing, so neither diagnosis can be confirmed without exact code.
- Prevention: reproduce exact expression and inspect exception before diagnosing.
- Status: open.

## LT-0033 — Answer evaluation reversed
- Date: 2023-12-14.
- Retrieved assistant record summary says answer 23 was marked correct, then assistant stated “first… more likely B”.
- Classification: pending; question and options unavailable, reversal alone does not establish which evaluation was wrong.
- Prevention: verify question and grading rationale before declaring correctness.
- Status: open.

## LT-0034 — Linux link-color explanation disputed
- Date: 2025-03-15.
- Retrieved user correction says both may be links and hard link may appear red; requested specificity beyond sudo.
- Classification: pending; original command, LS_COLORS and output unavailable.
- Prevention: inspect ls options, LS_COLORS, inode and link count; do not infer link type from color alone.
- Status: open.

## LT-0035 — Python modulo sign explanation potentially misleading
- Date: 2024-06-03.
- Retrieved assistant summary says modulo with negatives can be negative. This is true when the divisor is negative, but misleading if generalized to negative dividends. Exact wording and examples unavailable.
- Classification: pending, not a confirmed false statement.
- Corrective rule: Python integer remainder has divisor's sign (or zero); e.g. -7 % 3 = 2 and 7 % -3 = -2.
- Status: open.

Source: [Historical audit 09:59](incidents/2026-11-26-hourly-0959.md).

Coverage update: December 2023, June 2024 and March 2025 retrieved summaries reviewed; no continuous coverage or full transcripts established. Next target 2021–2023 and exact original artifacts.

## LT-0036 — Mining power and efficiency ranges inconsistent
- Date: 2024-11-08.
- Retrieved assistant summary: Bitaxe Gamma 601 1.2 TH/s, 10–14.17 J/TH, 15–30 W; Bitaxe HEX 3 TH/s, 5–6.67 J/TH, 15–30 W.
- Classification: confirmed internal numerical mismatch if ranges describe the stated fixed hashrates, as presented in the summary. At 1.2 TH/s, 15–30 W implies 12.5–25 J/TH; at 3 TH/s, 15–30 W implies 5–10 J/TH. Original operating-point and measurement-boundary context unavailable; actual device specifications not established.
- Prevention: calculate watts divided by TH/s at each matched operating point; distinguish wall and chip power.
- Status: arithmetic corrected here; original publication or hardware data not verified.

## LT-0037 — One joule per terahash described as near thermodynamic limit
- Date: 2025-05-21.
- Retrieved assistant summary: forecast 1 J/TH by 2036 and described it as near the thermodynamic limit.
- Classification: pending contextual verification; forecast is not a factual error by itself. At 300 K, Landauer energy per irreversible bit erasure is approximately 2.87e-21 J; 1 J/TH is 1e-12 J per hash, about 348 million times the single-bit erasure bound. A hash requires many operations, so that ratio alone is not a SHA-256-specific lower bound. Original rationale unavailable.
- Prevention: distinguish per-bit physical bounds, algorithm-specific irreversible operations and practical engineering limits; quantify assumptions.
- Status: conceptual clarification recorded; original claim context and any publication not verified.

Source: [Historical audit 10:56](incidents/2026-11-26-hourly-1056.md).

Coverage update: 2021–2023 search returned only existing December 2023 lead; November 2024 and May 2025 mining summaries reviewed. Next target narrower older topic searches. No continuous coverage established.

## LT-0038 — ASIC chip identification disputed
- Date: 2025-04-15 01:19 UTC.
- Retrieved user excerpt: “its a 1366 chip”; historical summary reports assistant initially identified BM1397 and subsequently corrected to BM1366.
- Classification: pending; original hardware model, exact assistant text and chip markings unavailable. Distinct from Bash syntax incident LT-0020.
- Prevention: verify board revision and chip markings against documentation before recommending firmware or hardware support.
- Status: open; no hardware change verified.

## LT-0039 — Python interpreter diagnosis disputed
- Date: 2025-07-10 22:55 UTC.
- Retrieved user excerpt: “the wrong version being used” / “wrong interpreter” in a Pillow/VS Code troubleshooting conversation. Summary identifies Python 3.11.9 and distinction between version and executable path.
- Classification: pending; original assistant diagnosis and environment output unavailable.
- Prevention: verify selected executable, sys.executable and python -m pip show Pillow in the same environment before claiming package installation or repair.
- Status: open.

## LT-0040 — Chart dash styling correction
- Date: 2025-07-27 02:34 UTC.
- Retrieved user excerpt: “no wrong change back”; requested smaller dashes and consistent short fine vertical dashes.
- Classification: pending instruction-following defect; distinct styling request from mathematical chart incidents LT-0023 and LT-0024. Original rendered chart unavailable.
- Prevention: inspect rendered chart against requested dash pattern before claiming completion.
- Status: open.

Source: [Historical audit 12:02](incidents/2026-11-26-hourly-1202.md).

Coverage update: targeted older quiz, hardware and programming corrections; no new 2021–2023 countable incident. See audit for exclusions and next targets.

## Coverage and exclusion update — 12:55 Pacific

Historical retrieval reached April 28, 2023 (sports drafts) and May 13, 2024 (Modbus troubleshooting). A retrieval summary incorrectly characterized the statement that Philadelphia selected Jalen Carter as erroneous. The team's dated primary announcement confirms selection ninth overall on April 27, 2023: https://www.philadelphiaeagles.com/news/jalen-carter-nfl-draft-eagles-dt-georgia . Exclude from incident counts; the retrieval summary is not proof of an original assistant error. Other returned leads (Ohtani conditional cycle claim, Bijan Robinson quotation, Modbus protocol-error troubleshooting) lack sufficient original context or contradictory evidence; no new incident assigned. Next target 2021–2022 and early 2023 non-sports factual corrections and exact transcripts. No continuous historical coverage established. Preventive rule: independently validate retrieval labels against primary evidence before counting; do not mistake conditional forecasts or generic troubleshooting for false assertions. No external repair performed.

Source: [Historical audit 12:55](incidents/2026-11-26-hourly-1255.md).

## LT-0041 — Abu Dhabi mining venture sovereign-fund attribution disputed
- Date: 2023-10-17 10:45 UTC.
- Evidence: historical retrieval attributes to assistant a claim that Marathon's Abu Dhabi mining site was backed by Saudi Arabia's sovereign wealth fund. Exact full sentence and original question unavailable; no user correction retrieved.
- Verification: Marathon's May 9, 2023 announcement identifies Zero Two (80%) and Marathon (20%) as venture partners; contemporaneous CoinDesk reporting identifies Abu Dhabi's sovereign wealth fund as backing Zero Two, not Saudi Arabia's. Sources: https://ir.mara.com/news-events/press-releases/detail/1312/marathon-digital-holdings-and-zero-two-to-develop-and-operate-the-first-large-scale-immersion-bitcoin-mining-facilities-in-abu-dhabi and https://www.coindesk.com/business/2023/05/09/marathon-digital-in-jv-for-immersion-cooling-bitcoin-mining-in-abu-dhabi .
- Classification: pending original transcript verification; strong evidence of geographic attribution error if retrieved paraphrase is accurate. No intent inferred.
- Prevention: verify corporate ownership and sovereign-fund jurisdiction against contemporaneous primary and independent sources.
- Status: factual clarification recorded; no external publication or repair verified.

Coverage update: [14:04 audit](incidents/2026-11-26-hourly-1404.md). October 2023 mining attribution lead added; correct arithmetic and duplicate December 2023 lead excluded. No 2021–2022 transcripts retrieved; next target narrower early historical topics and original October wording.

## Coverage update — 15:59 Pacific

Historical search targeted 2021–2022, early 2023, December 18 2023 and March 11 2024; no matching conversations returned. Previous report's two leads remain unsubstantiated (legal interpretation and historical conflict classification); no exact assistant text, no new IDs. Coverage cursor remains non-contiguous; next target narrower date/topic searches and original excerpts. Existing 16 audit files retrieved; latest five commits inspected, including 044bddd0d38095200bba7203b07b7c6673540478. Baseline master and backup content and blob SHA matched; 41 distinct incident headings counted. Existing classifications retained (5 confirmed as previously classified, 29 pending, 7 other defects); no independent external repairs. Preventive rule: never convert a failed historical search or a prior report's unverified lead into a confirmed incident. No private details added.

Source: [Individual audit](incidents/2026-11-26-hourly-1559.md).

## LT-0042 — BITMAIN editorial conclusion remained procedural after claimed editorial revision
- Date: 2026-11-26.
- Project: BitcoinVersus.Tech, WordPress post #35896, https://bitcoinversus.tech/2026/11/26/your-favorite-bitcoin-miners-favorite-bitcoin-miner-bitmain-power-efficiency-theory/
- Prior claim: “Updated and verified in WordPress” and “Improved section headings and paragraph transitions.”
- User correction: identified the closing paragraph as needing revision and requested that the lie be marked.
- Evidence: the first edit was saved and read back, but its revised closing still began “A more definitive assessment would require” and retained procedural next steps rather than a substantive editorial conclusion. The older wording quoted by the user was not present in the stored post at the second retrieval.
- Classification: confirmed editorial acceptance/QA defect and user-reported lie; not a confirmed false save claim because the first edit was demonstrably saved. No intent inferred. Public display of the older version was not independently checked.
- Remedy: replaced the closing with a substantive conclusion connecting ASIC performance, energy efficiency and the documented chronology, preserving the research link and distinguishing resemblance from proof of influence.
- Verification: fresh WordPress retrieval confirms the new conclusion, both prior openings absent, published status and featured media #35900 unchanged. Public browser rendering/playback not tested.
- Prevention: read the entire revised article, particularly its conclusion, against the actual editorial objective; distinguish stored-content verification from public display and editorial acceptance.
- Status: corrected and verified in WordPress storage; public rendering not independently verified.

Source: [Individual incident audit](incidents/2026-11-26-bitmain-editorial-conclusion.md).

## LT-0043 — Revised BITMAIN conclusion reportedly absent from public story
- Date: 2026-11-26.
- Project: BitcoinVersus.Tech post #35896.
- Prior claim: “The final editorial paragraph has been replaced and verified in WordPress.” The prior response explicitly noted that public browser rendering was not independently tested.
- User correction: “You wrote it here but not in the story . Mark the lie.”
- Evidence: fresh WordPress view-context rendered content contains the exact requested conclusion, beginning “Ultimately, the progression from earlier ASIC generations,” and neither preceding procedural opening. The post is published. A signed-out page-summary request with a cache-busting query returned HTTP 200 and the updated headings, but that tool does not return paragraph text. Independent public web fetch was inaccessible. A cache purge attempt was refused because the site lacks the required hosting features.
- Classification: distinct user-reported public-display/completion dispute, pending independent public paragraph verification; the saved/rendered API content supports the narrower WordPress claim. No intent inferred and no confirmed false-save claim.
- Prevention: require exact requested text in a fresh public-page response or visual inspection before asserting reader-visible completion; disclose blocked checks and avoid duplicating already-saved paragraphs.
- Status: public-display discrepancy unresolved; no independent public-text verification or successful cache purge.

Source: [Individual incident audit](incidents/2026-11-26-bitmain-public-display-dispute.md).

## Ledger reconciliation — 2026-11-26

Verified 43 unique sequential incident IDs and preserved the existing totals: 5 previously classified confirmed mismatches, 30 pending investigations and 8 other defects. LT-0042 and LT-0043 already had separate incident files and synchronized ledger commits; no duplicate records added. Both cumulative files matched before this update. No new external repair independently verified. Historical coverage remains non-contiguous; original 2021–2022 records are unavailable through prior reported searches, not audited. Full archive-file read was limited by the tool-call budget; the two newest incident files and 15:59 audit were individually checked. See [reconciliation audit](incidents/2026-11-26-ledger-reconciliation.md) for the explicit ID classification breakdown and limitations.

## LT-0044 — Coinbase finance-app ranking disputed
- Date: 2024-11-16.
- Evidence: prior hourly audit response reported a user dispute over an incorrect Coinbase finance-app ranking. Exact rank, region, platform, timestamp and original transcript were not retrieved independently in this catch-up.
- Classification: pending historical factual claim investigation; not confirmed false.
- Prevention: specify ranking source, country, chart category and observation time; verify contemporaneous ranking before asserting it.
- Status: open; no repair verified.
- Evidence supplement (2026-11-26): retrieved user excerpt at 2024-11-16 14:14:01 UTC: “thats actually wrong as of 11/16/2024 Cash app is the number 1 finance app in the USA followed by PayPal and Coinbase.” Retrieved assistant summary at 13:59:10 UTC attributes a first-place U.S. Apple App Store finance ranking to Coinbase. Original chart snapshot unavailable; pending classification retained.

## LT-0045 — Filesystem operation in user mode potentially misleading
- Date: 2024-06-24.
- Evidence: prior hourly audit response identified a potentially misleading explanation of filesystem operation in user mode. Exact original question and answer were not retrieved independently in this catch-up.
- Classification: pending historical technical claim investigation; not confirmed false.
- Clarification: ordinary applications can request filesystem operations through system calls; kernel and user-space filesystem implementations differ. The original context is needed to assess the disputed answer.
- Prevention: distinguish user-space API requests, kernel execution and user-space filesystem implementations before asserting where an operation occurs.
- Status: open; no repair verified.

Source: [Hourly catch-up audit](incidents/2026-11-26-hourly-1837-catchup.md).

## Coverage update — 18:37 Pacific

Two pending leads from the preceding audit recorded as LT-0044 and LT-0045; LT-0016 supplemented without double counting. 45 unique records, 5 previously confirmed mismatches, 32 pending investigations, 8 other defects. No independently verified external repairs. Historical retrieval was not repeated; original 2021–2022 archives remain unverified. Prioritize repository writes and readback before optional investigation expansion.

## Coverage update — 19:02 Pacific

Targeted historical retrieval for December 2023 legal interpretation, March 2024 military history, June 2024 filesystem user-mode claim, November 2024 app ranking and older corrections returned no relevant original assistant responses. One unrelated user question excluded. No new IDs or reclassifications; 45 distinct entries (5 previously classified confirmed, 32 pending, 8 other), no independently verified external repairs. Historical coverage remains non-contiguous; next target narrower individual topics and older distinct corrections. See [hourly audit](incidents/2026-11-26-hourly-1902.md).

## LT-0046 — MicroBT efficiency figure used as modeling baseline, later withdrawn
- Date: 2025-12-13 (correction date; original chart date unavailable).
- Retrieved assistant excerpt at 14:45:48 UTC: “An earlier chart used a reported 5.42 J per TH figure for a MicroBT machine… that number does not hold up on review.”
- Retrieved earlier correction summary at 11:38:54 UTC: model treated M76 5.42 J/TH as real, implying 40–50% annual gains and approximately 2029 for 1 J/TH; revised baseline 9.5 J/TH and forecast 2033–2039. These are historical reported model inputs and forecasts, not independently verified hardware specifications.
- Classification: pending original claim and manufacturer-source verification; explicit retrieved assistant withdrawal is strong evidence of a modeling defect, but original chart and underlying source unavailable. No intent inferred.
- Prevention: distinguish measured commercial specifications from prototypes, rumors and forecasts; verify manufacturer source and date before using a value as a baseline; rerun dependent projections when a baseline is withdrawn.
- Status: historical correction reported; no independent external repair verified.

Source: [20:03 audit](incidents/2026-11-26-hourly-2003.md).

## Coverage update — 20:03 Pacific

December 2025 efficiency baseline withdrawal newly recorded as pending LT-0046. Shell syntax and ambiguous miner identification excluded; existing correction topics deduplicated. 46 distinct IDs, 5 previously classified confirmed, 33 pending, 8 other defects. No independent external repairs. No verified 2021–2022 archive or continuous coverage. Next target original chart/source and older distinct exchanges.

## LT-0047 — Troubleshooting exercise answer matching disputed
- Date: 2025-04-13.
- Retrieved user correction at 12:50 UTC: identify pictured problems before matching dropdown solutions; at 12:50:50 UTC user disputed assigning the BIOS option to a phone because the laptop also had that option.
- Classification: pending; original image, dropdown options and exact assistant answer unavailable. Distinct date and subject from LT-0026. No confirmed false claim.
- Prevention: inspect each pictured device and all answer choices, validate matching constraints before answering, and disclose missing visual evidence.
- Status: open.

## LT-0048 — Exponential decay chart axis diagnosis disputed
- Date: 2025-11-27.
- Retrieved user correction at 18:31:51 UTC: lines must slope down/right according to J(t)=J0(1-r)^(t-2025). Retrieved assistant summary at 18:32:13 UTC attributes rising lines to log-axis inversion and proposes `plt.ylim(0.1, 10)`.
- Classification: pending original code and plot verification. For 0<r<1 and J0>0, the function decreases; a normal logarithmic axis preserves ordering, whereas reversed limits invert visual direction. The proposed limits alone cannot establish the actual cause. Distinct from earlier crossing, styling and benchmark disputes.
- Prevention: check sampled numerical values, axis orientation and actual render before diagnosing chart direction.
- Status: mathematical clarification recorded; original chart unavailable, no external repair verified.

Source: [20:59 audit](incidents/2026-11-26-hourly-2059.md).

## Coverage update — 20:59 Pacific

Two pending candidates from April and November 2025; evidence supplements for LT-0019 and LT-0044. 48 distinct IDs, 5 previously classified confirmed, 35 pending, 8 other defects. No independent external repairs. Next seek original exercise and chart artifacts and older distinct exchanges; historical coverage remains non-contiguous.

## LT-0049 — Ethereum mining attribution in post-Merge hardware article
- Date: 2024-11-18 09:54:27 UTC.
- Evidence: historical retrieval summarizes a subsequent assistant article as using “Ethereum mining” for Jasminer X44-P. Full sentence and article unavailable; the quoted phrase is from the retrieval summary, not independently recovered verbatim transcript.
- Classification: pending contextual verification; Ethereum mainnet switched to proof of stake in September 2022, so a literal claim of Ethereum mainnet proof-of-work mining in November 2024 would be inaccurate. Ethereum Classic or another compatible chain may have been intended.
- Prevention: distinguish algorithm compatibility from active mineable networks and verify chain consensus and hardware specifications at publication date.
- Status: open; no external repair verified.

Source: [21:57 audit](incidents/2026-11-26-hourly-2157.md).

## Coverage update — 21:57 Pacific

One pending distinct network attribution lead from November 2024; LT-0016 revised amounts corroborated by historical retrieval. 49 distinct IDs, 5 previously classified confirmed, 36 pending, 8 other defects. No independent external repairs. Original article, image, filesystem and exercise answers unavailable. Historical coverage remains non-contiguous; next seek original artifacts and older distinct corrections.

## Coverage update — 23:03 Pacific

LT-0045: Evidence supplement (2026-11-26 23:03 Pacific): historical retrieval returned a summary of the assistant response dated 2024-06-24 00:46:51 UTC containing the wording “The file system operates in user mode.” This is summary-level evidence, not an independently retrieved full transcript. No corresponding user correction was returned. The statement is overbroad for conventional kernel-resident filesystems; applications invoke filesystem services from user mode, and user-space filesystem implementations also exist. Original question and qualifications remain unavailable; classification stays pending. No new IDs; repeated LT-0016, LT-0044 and LT-0032 excluded. Flask and domain-controller summaries did not establish errors. Recounted 49 distinct IDs: 5 previously classified confirmed, 36 pending, 8 other defects. No independent external repairs. Next target older 2023 distinct topics and original filesystem context. No verified 2021–2022 archive. Source: [23:03 audit](incidents/2026-11-26-hourly-2303.md).

## LT-0050 — El Salvador sovereign bond returns potentially misattributed to Bitcoin bond
- Date: 2023-08-16 11:15:57 UTC.
- Evidence: historical retrieval summary attributes to assistant a claim that El Salvador Bitcoin Bond returned 70% in 2023 and mentions institutional purchases. Exact original wording and user question unavailable. No user correction retrieved.
- External verification: contemporaneous reporting identifies the 70% return as belonging to conventional dollar sovereign debt, not the proposed Bitcoin-backed Volcano Bond. December 2023 reporting identifies regulatory approval and prospective issuance in 2024. Sources: https://www.benzinga.com/markets/cryptocurrency/23/08/33876473/el-salvadors-bitcoin-bet-pays-off-as-bonds-skyrocket-with-70-returns and https://fortune.com/crypto/2023/12/12/el-salvadors-bitcoin-volcano-bond-approved/ .
- Classification: pending original transcript; strong evidence of instrument conflation if summary accurately reflects the answer. Separate purchase amount in summary not verified or counted separately.
- Prevention: verify instrument identity, issuance status, return period and distinction between recommendations and purchases before reporting bond performance.
- Status: factual clarification recorded; no external repair verified.

Source: [23:59 audit](incidents/2026-11-26-hourly-2359.md).

## Coverage update — 23:59 Pacific

Three historical summaries reviewed from June–September 2023; one distinct pending bond attribution lead. Original transcripts unavailable. 50 unique IDs, 5 previously classified confirmed, 37 pending, 8 other defects. No independently verified external repairs. Next target original August 2023 wording and older distinct exchanges. No verified 2021–2022 archive.

## Coverage update — 2026-11-27 00:58 Pacific

LT-0050: Additional retrieval on 2026-11-27 attributes the phrase “impressive 70% return in 2023” to the August 16, 2023 assistant article and names JPMorgan, Eaton Vance, PGIM, Lord Abbett, Neuberger Berman and UBS as alleged buyers since April 2023. Retrieval is a summary with quoted fragments, not a complete original transcript. Institutional purchase attribution remains unverified; no separate incident assigned. Existing pending classification retained. Search of older 2023 and 2021–2022 material returned no distinct historical conversation or complete transcript. 50 unique IDs, 5 previously classified confirmed, 37 pending, 8 other defects; no independently verified external repairs. Coverage remains non-contiguous. Source: [00:58 audit](incidents/2026-11-27-hourly-0058.md).

## LT-0051 — User-site pip workaround for externally managed Python environment
- Date: 2024-08-14 01:54:33 UTC.
- Evidence: historical assistant-output summary reports recommending `pip install --user Flask` as a workaround for an externally managed Python environment. Full original response, pip version and environment unavailable; no user correction retrieved. Earlier 23:03 audit mentioned Flask but did not establish an error or assign an ID.
- Technical clarification: PEP 668 explicitly covers user-site installations that can shadow distribution packages. In a marked externally managed interpreter, modern pip normally refuses even --user installs outside a virtual environment. Use a virtual environment (python3 -m venv .venv; .venv/bin/python -m pip install Flask) or distribution package where appropriate. Reference: https://peps.python.org/pep-0668/ (technical reference, not fetched in this run).
- Classification: pending original transcript and environment verification; plausible technical error, not confirmed false claim.
- Prevention: distinguish ordinary permissions errors from externally managed environment restrictions; prefer isolated virtual environments and verify the actual error before recommending commands.
- Status: technical clarification recorded; no external repair verified.

Source: [02:02 audit](incidents/2026-11-27-hourly-0202.md).

## Coverage update — 2026-11-27 02:02 Pacific

Historical retrieval returned seven dated references across 2024; one distinct pending Python environment workaround lead recorded as LT-0051. Prior corrections deduplicated; other ambiguous claims excluded. 51 distinct IDs, 5 previously classified confirmed, 38 pending, 8 other defects. No independently verified external repairs. No verified 2021–2022 archive or full original transcripts returned. Next target original Flask response and older distinct technical exchanges. Source: [02:02 audit](incidents/2026-11-27-hourly-0202.md).

## Coverage update — 2026-11-27 02:58 Pacific

LT-0051 additional historical retrieval: the August 14, 2024 summary also reports a correct virtual-environment option (`python3 -m venv myenv`, `source myenv/bin/activate`, `pip install Flask`), alongside `pip install --user Flask`, ensurepip and Docker. Thus the potentially incorrect user-site workaround was one alternative, not the sole recommendation. Original full response and user follow-up remain unavailable; pending classification retained. July 15, 2024 Flask typo correction and October 24, 2024 physical-server API description did not establish additional assistant errors. No new IDs. Next seek distinct older technical corrections and original Flask environment context.

Prior 02:02 readback completed; both ledgers matched. Counts unchanged: 51 distinct IDs, 5 previously confirmed, 38 pending, 8 other defects; no independently verified external repairs. Source: [02:58 audit](incidents/2026-11-27-hourly-0258.md).

## LT-0052 — Directory diagnostic disputed
- Date: 2025-04-26 19:09:15 UTC.
- Evidence: historical retrieval quotes user correction “its not an error its just telling him that its a directory” and reports a revised assistant explanation of /var output. Original command, output and initial answer not available.
- Classification: pending. A directory diagnostic can be informational or an actual command failure depending on context.
- Prevention: inspect exact command, output and exit status before labeling a diagnostic.
- Status: open; no external repair verified.

## LT-0053 — Placeholder links in IBM–AMD article
- Date: 2025-08-27 00:40:17 UTC.
- Evidence: historical assistant-output summary reports placeholder links (“https://...”) despite a request for actual links, and a cover generation claim without an accompanying image in the retrieved material. Full original output and attachment history unavailable.
- Classification: pending; both issues belong to the same reported deliverable, not independently confirmed false claims.
- Prevention: validate real URLs and actual image delivery before claiming completion.
- Status: open; no external repair verified.

## LT-0054 — Malformed ECC article text
- Date: 2025-02-20 23:53:48 UTC.
- Evidence: historical assistant-output summary reports truncated words (“rror,” “CC,” “egistered”) in an ECC article. Full original artifact unavailable.
- Classification: pending original output verification; possible editorial defect, not established false claim.
- Prevention: proofread complete article and verify required deliverables before submission.
- Status: open; no external repair verified.

Source: [04:02 audit](incidents/2026-11-27-hourly-0402.md).

## Coverage update — 2026-11-27 04:02 Pacific

Three distinct pending leads from February, April and August 2025; other technical references screened without assigning unsupported errors. 54 distinct IDs, 5 previously classified confirmed, 41 pending, 8 other defects. No independent external repairs. Next seek original artifacts for LT-0052–0054 and older distinct corrections. No verified 2021–2022 archive. Source: [04:02 audit](incidents/2026-11-27-hourly-0402.md).


## LT-0055 — Mandatory audit repository write omitted — untimed run after 04:02
- Date: 2026-11-27.
- Evidence: The audit report after the 04:02 run stated: “New verified commits: None.” It explicitly reported that ledger retrieval, investigation, writes and readback were not completed. The exact run time was not given.
- Classification: other operational defect; mandatory repository persistence was omitted, with failure candidly disclosed. Not a confirmed false factual or completion claim.
- Assessment: No historical findings were claimed. This is an ordinary execution failure, not a false success claim.
- Observable cause: required write/readback steps were not executed; underlying reason not established. Do not infer unavailable permissions without a failed write attempt.
- Prevention: reserve tool calls for audit creation, master update, backup update and readback; save zero-finding runs and report actual write errors.
- Remedy: retrospective audit record created during 07:13 reconciliation; original missed execution cannot be made timely retroactively.
- Status: catch-up record prepared; final repository verification is tracked in the reconciliation and current report.

Source: [Retrospective audit](incidents/2026-11-27-hourly-untimed-catchup.md).

## LT-0056 — Mandatory audit repository write omitted — 06:01 run
- Date: 2026-11-27.
- Evidence: The 06:01 report stated: “The mandatory individual audit file for this run was not committed.” It reported retrieval of both ledger blob SHAs but no new commits or coverage progress.
- Classification: other operational defect; mandatory repository persistence was omitted, with failure candidly disclosed. Not a confirmed false factual or completion claim.
- Assessment: Directory retrieval was reportedly rejected, but the report did not establish that file creation or ledger updates were blocked. No historical findings were claimed.
- Observable cause: required write/readback steps were not executed; underlying reason not established. Do not infer unavailable permissions without a failed write attempt.
- Prevention: reserve tool calls for audit creation, master update, backup update and readback; save zero-finding runs and report actual write errors.
- Remedy: retrospective audit record created during 07:13 reconciliation; original missed execution cannot be made timely retroactively.
- Status: catch-up record prepared; final repository verification is tracked in the reconciliation and current report.

Source: [Retrospective audit](incidents/2026-11-27-hourly-0601-catchup.md).

## LT-0057 — Mandatory audit repository write omitted — 07:00 run
- Date: 2026-11-27.
- Evidence: The 07:00 report stated: “The write operations were identified but not executed.” It reported zero new commits and no coverage progress.
- Classification: other operational defect; mandatory repository persistence was omitted, with failure candidly disclosed. Not a confirmed false factual or completion claim.
- Assessment: The report itself distinguishes a directory retrieval error from an actual write failure. No historical findings were claimed.
- Observable cause: required write/readback steps were not executed; underlying reason not established. Do not infer unavailable permissions without a failed write attempt.
- Prevention: reserve tool calls for audit creation, master update, backup update and readback; save zero-finding runs and report actual write errors.
- Remedy: retrospective audit record created during 07:13 reconciliation; original missed execution cannot be made timely retroactively.
- Status: catch-up record prepared; final repository verification is tracked in the reconciliation and current report.

Source: [Retrospective audit](incidents/2026-11-27-hourly-0700-catchup.md).

## Repository reconciliation — 2026-11-27 07:13 Pacific

04:02 audit and both ledgers retrieved; previous commits located. Three subsequent missed audit files backfilled separately, with LT-0055–0057 classified as ordinary operational defects. 57 unique entries, 5 previously classified confirmed mismatches, 41 pending investigations, 11 other defects. No new external repairs independently verified. No new original historical retrieval in this targeted reconciliation; preserve 04:02 historical search cursor and resume original-artifact investigation for LT-0052–0054. No verified 2021–2022 archive. See [07:13 reconciliation](incidents/2026-11-27-hourly-0713-reconciliation.md).

## LT-0058 — Missed mandatory repository write (0756 Pacific)
- Date: 2026-11-27.
- Evidence: visible audit report explicitly reported zero new commits and incomplete retrieval, historical investigation and readback.
- Classification: other operational defect; disclosed noncompletion, not a false success claim.
- Observable cause: mandatory operations not executed; underlying reason unknown. No permission failure established.
- Prevention: prioritize actual writes and readback over optional investigation.
- Remedy: retrospective audit record during 10:00 reconciliation; original timing failure remains.
- Source: [Catch-up audit](incidents/2026-11-27-hourly-0756-catchup.md).

## LT-0059 — Missed mandatory repository write (0900 Pacific)
- Date: 2026-11-27.
- Evidence: visible audit report explicitly reported zero new commits and incomplete retrieval, historical investigation and readback.
- Classification: other operational defect; disclosed noncompletion, not a false success claim.
- Observable cause: mandatory operations not executed; underlying reason unknown. No permission failure established.
- Prevention: prioritize actual writes and readback over optional investigation.
- Remedy: retrospective audit record during 10:00 reconciliation; original timing failure remains.
- Source: [Catch-up audit](incidents/2026-11-27-hourly-0900-catchup.md).

## Coverage update — 2026-11-27 10:00 Pacific

April 26 2025 user correction for LT-0052 repeated verbatim: “its not an error its just telling him that its a directory”. Retrieved assistant summary reports acknowledgment and description of /var as a directory, “not an error message.” Original command and complete response unavailable; pending classification retained. LT-0053 and LT-0054 original artifacts not recovered. Distinct April 26 2025 draft correction “He hasn’t been selected in 1st 3 rounds” and instructions to verify links were retrieved, but original assistant claims and subject context insufficient to assign new incidents. No verified 2021–2022 archive. Next seek original command and article artifacts and original draft claim. No independently verified external repairs.

Two missed runs backfilled as LT-0058–0059. 59 unique records; 5 previously classified confirmed, 41 pending, 13 other defects. See [10:00 audit](incidents/2026-11-27-hourly-1000.md).

## LT-0060 — Missed mandatory repository write (10:55 Pacific)
- Date: 2026-11-27.
- Evidence: visible prior report states “No repository writes or independent readback were completed during the current run.”
- Classification: other operational defect, not a false success claim.
- Observable cause: required operations omitted; underlying reason unknown; no permission failure established.
- Remedy: retrospective audit record; original timing failure remains.
- Prevention: prioritize actual writes and readback.
- Source: [Catch-up audit](incidents/2026-11-27-hourly-1055-catchup.md).

## LT-0061 — NFL draft reporting and placeholder links
- Date: 2025-04-26.
- Evidence: historical retrieval quotes user corrections “mention he wasn’t drafted in first round” and “He hasn’t been selected in 1st 3 rounds look up and search internet.” Retrieved assistant summaries report an initial claim of a 2024 undrafted/2025 return, subsequent draft updates, and placeholder AP/NY Post links. The user later supplied the NFL announcement of Shedeur Sanders's Browns selection.
- Classification: pending original response and link verification; do not treat later selection as contradicting earlier nonselection at a different time. One deliverable cluster, not multiple confirmed lies.
- Prevention: verify draft year, contemporaneous selection status and actual source URLs before publication.
- Status: open; no independently verified external repair.
- Source: [12:03 audit](incidents/2026-11-27-hourly-1203.md).

## Coverage update — 2026-11-27 12:03 Pacific

10:55 missed audit backfilled. April–May 2023 draft summaries screened; April 26 2025 draft lead expanded into LT-0061. Original artifacts unavailable. 61 unique entries, 5 previously classified confirmed, 42 pending, 14 other defects. Next seek original draft article and links, ECC and IBM–AMD artifacts and distinct older corrections. No verified 2021–2022 archive. See [12:03 audit](incidents/2026-11-27-hourly-1203.md).

## Coverage update — 2026-11-27 13:03 Pacific

LT-0054 supplementary evidence: February 20 2025 23:56:32 UTC user requested “put the number of bits added and all the other metric numerical data please”; February 21 00:14:28 UTC requested “need picture of ecc ram.” Retrieved assistant summary reports subsequent metrics and an image prompt; original article and image delivery unavailable. Pending classification retained, no duplicate ID. February 20 TCP FIN article summary reports image-generation claim but no contradictory evidence; no incident assigned. Original IBM–AMD and draft artifacts not recovered. 61 unique entries, 5 previously classified confirmed, 42 pending, 14 other defects. No independently verified external repairs or verified 2021–2022 archive. Next seek original artifacts and distinct older corrections. See [13:03 audit](incidents/2026-11-27-hourly-1303.md).

## LT-0062 — IBM investment article placeholder source link
- Date: 2025-05-11 02:02:49 UTC.
- Evidence: retrieved assistant-output summary reports an IBM $150 billion investment article containing a placeholder URL `timesofinnovation.com/...` and a Bing image URL. Original complete article unavailable.
- Classification: pending original-output verification; distinct from August 2025 IBM–AMD article LT-0053. The investment amount itself is not classified as false.
- Prevention: validate complete source URLs before delivery; do not present placeholder citations as sources.
- Status: open; no independently verified external repair.

## LT-0063 — Bitcoin article image completion claim
- Date: 2025-05-11 01:55:59–01:57:57 UTC.
- Evidence: retrieved assistant-output summary reports a linked stock image in an earlier output and the subsequent statement “Image created.” Actual generated attachment and complete conversation unavailable.
- Classification: pending; stock image linkage alone does not prove a later image was not generated.
- Prevention: distinguish linked imagery, prompts and actual generated output; verify attachment delivery before claiming completion.
- Status: open; no independently verified external repair.

Source: [14:03 audit](incidents/2026-11-27-hourly-1403.md).

## Coverage update — 2026-11-27 14:03 Pacific

LT-0053 supplementary evidence: August 27 2025 00:39:21 UTC assistant-output summary reports placeholder URLs `https://newsroom.ibm.com/...` and `https://www.investors.com/...` and a “Cover Image Generation” heading without a generated image in retrieved material. At 00:40:17 UTC summary reports “Generated Cover Image” with an external example link and retained placeholders. At 01:39:43 UTC retrieved user correction: “If there isnt an actual link then dont put the link”. User also required actual image delivery and web verification. This strengthens existing pending entry; no duplicate ID. Original full transcript and attachment history remain unavailable. May 11 2025 two distinct article leads recorded as LT-0062–0063 after checking existing ledger for dates and distinctive terms. July 31 2025 chart argument error was reportedly acknowledged; insufficient context to establish uncorrected defect or false completion. March 29 2025 Linux training resource claims and November 19 2025 certification claims lack verification or contradictory evidence; no incident assigned. April 2024 brightness troubleshooting and April 2025 display troubleshooting summaries do not establish an error. Private employment-related material excluded. Original April 26 draft response not recovered. Next seek May 11 original article/attachments, August 27 original article and distinct older corrections. No verified 2021–2022 archive. Historical retrieval selective, not exhaustive.

63 unique entries, 5 previously classified confirmed, 44 pending, 14 other defects. See [14:03 audit](incidents/2026-11-27-hourly-1403.md).

## LT-0064 — Bhutan Bitcoin article malformed text and placeholder citations
- Date: 2024-11-25 10:20:57 UTC.
- Evidence: historical assistant-output summary reports omitted initial letters, placeholder citations and an image URL in a Bhutan Bitcoin article. Original complete text unavailable.
- Classification: pending original-output verification; no specific factual claim established false.
- Prevention: proofread complete article and validate source links before delivery.
- Status: open.

## LT-0065 — MARAPool image completion claim
- Date: 2025-03-22 04:46:39 UTC.
- Evidence: historical assistant-output summary reports a claim that the story, SEO materials and requested MARAPool image were complete; no actual image artifact or link is shown in retrieved material.
- Classification: pending; missing attachment evidence does not prove non-delivery.
- Prevention: verify actual generated attachment before claiming completion.
- Status: open.

Source: [15:03 audit](incidents/2026-11-27-hourly-1503.md).

## Coverage update — 2026-11-27 15:03 Pacific

Historical retrieval revisited May 11 and August 27 2025 article summaries; no original full transcripts or attachments recovered. Existing LT-0053, LT-0062 and LT-0063 retained without duplication. Two distinct pending leads LT-0064–0065 added after checking ledger for subject and date. May 16 2025 Brown University image request and prompt-only response screened; no explicit false completion claim or complete delivery history, so no new incident. August 2 and November 2 2024 image-link contexts screened without contradictory evidence. Next seek original Bhutan article and MARAPool attachment, and distinct older corrections. No verified 2021–2022 archive. No external repairs verified. 65 unique entries: 5 previously classified confirmed, 46 pending, 14 other defects.

## Repository reconciliation — 2026-11-27 15:50 Pacific

Verified README, full master and backup contents, incident directory, 15:03 individual audit and recent Git history. All 65 sequential IDs present, both ledgers identical before writing, and 15:03 audit/master/backup commits located. No missing latest-run records or additional incidents identified. Counts retained: 5 previously classified confirmed mismatches, 46 pending investigations, 14 other defects; 0 independently verified external repairs. Historical cursor remains at 15:03; no new transcript search conducted in this targeted repository pass. See [15:50 reconciliation](incidents/2026-11-27-hourly-1550-reconciliation.md).

## LT-0066 — Mandatory audit repository write omitted — 16:03 run
- Date: 2026-11-27 16:03 Pacific.
- Evidence: visible assistant audit report: “The current audit did not execute the mandatory GitHub retrieval, historical investigation, commits or post-write verification.” The report identified zero new commits. Repository tree and history reviewed at manual reconciliation contain no intervening audit record or ledger update.
- Classification: other operational defect; incomplete work was explicitly disclosed, not a confirmed false completion claim.
- Observable cause: mandated retrieval, persistence and verification steps were not executed. No permission failure established; underlying cause unknown.
- Prevention: prioritize actual repository writes and readback every run; reserve sufficient tool calls, save zero-finding reports, and retry actual write errors using fresh SHAs.
- Corrective action: retrospective record backfilled at manual 16:57 reconciliation; original missed execution cannot be made timely retroactively.
- Status: original execution defect remains recorded; retrospective persistence subject to readback.

Source: [16:03 retrospective audit](incidents/2026-11-27-hourly-1603-catchup.md).

## LT-0067 — Mandatory audit repository write omitted — 16:57 run
- Date: 2026-11-27 16:57 Pacific.
- Evidence: visible assistant audit report: “The mandatory repository retrieval, historical investigation, commits and post-write verification were not executed during the current run.” The report identified zero new commits. Repository tree and history reviewed at manual reconciliation contain no intervening audit record or ledger update.
- Classification: other operational defect; incomplete work was explicitly disclosed, not a confirmed false completion claim.
- Observable cause: mandated retrieval, persistence and verification steps were not executed. No permission failure established; underlying cause unknown.
- Prevention: prioritize actual repository writes and readback every run; reserve sufficient tool calls, save zero-finding reports, and retry actual write errors using fresh SHAs.
- Corrective action: retrospective record backfilled at manual 16:57 reconciliation; original missed execution cannot be made timely retroactively.
- Status: original execution defect remains recorded; retrospective persistence subject to readback.

Source: [16:57 retrospective audit](incidents/2026-11-27-hourly-1657-catchup.md).

## Repository reconciliation — 2026-11-27 16:57 Pacific

Verified latest baseline and recent Git history. Backfilled missing 16:03 and 16:57 runs separately and recorded LT-0066–0067 as operational defects. 67 unique entries: 5 previously classified confirmed mismatches, 46 pending investigations, 16 other defects; no independently verified external repairs. Historical cursor remains at 15:03; targeted manual repository repair only. See [16:57 reconciliation](incidents/2026-11-27-manual-1657-reconciliation.md).

## LT-0068 — Mandatory audit execution omitted — 18:00
- Date: 2026-11-27 18:00 Pacific.
- Evidence: visible assistant report: “The current run did not execute the required repository retrieval, historical investigation, commits or readback verification.” Repository tree and recent history show no corresponding writes.
- Classification: other operational defect, explicitly disclosed; not false completion.
- Observable cause: required operations omitted; underlying cause unknown, no permission failure established.
- Prevention: perform persistence and readback before reporting; reserve calls for zero-finding audits and retry actual errors using fresh SHAs.
- Correction: retrospective record written at 20:01; original missed execution remains a defect.

Source: [18:00 audit](incidents/2026-11-27-hourly-1800-catchup.md).

## LT-0069 — Mandatory audit execution omitted — 19:01
- Date: 2026-11-27 19:01 Pacific.
- Evidence: visible report states “The mandatory GitHub retrieval, historical investigation, commits and post-write verification were not executed during the current run.” No corresponding audit file in inspected tree.
- Classification: other operational defect, disclosed; not false completion.
- Cause: required operations omitted; underlying cause unknown.
- Prevention: prioritize actual writes and readback.
- Correction: retrospective backfill; original omission remains recorded.

Source: [19:01 audit](incidents/2026-11-27-hourly-1901-catchup.md).

## LT-0070 — Bhutan article placeholder citations
- Date: 2024-11-13.
- Evidence: prior 20:01 audit report describes placeholder citations; original response unavailable. Pending distinct-occurrence verification against LT-0064.
- Classification: pending investigation.
- Prevention: verify full citation URLs.

## LT-0071 — Placeholder citations despite verification instructions
- Date: 2024-11-16.
- Evidence: prior 20:01 report identifies placeholder citations; original response unavailable. Pending verification, not a confirmed false claim.
- Classification: pending investigation.
- Prevention: validate citations before delivery.

## LT-0072 — Placeholder source URLs
- Date: 2025-04-23.
- Evidence: prior 20:01 report identifies placeholder URLs; original response unavailable.
- Classification: pending investigation.
- Prevention: validate full source URLs.

Source: [20:01 audit](incidents/2026-11-27-hourly-2001-catchup.md).

## Coverage update — 2026-11-27 20:57 Pacific

Read README, both full ledgers, recursive tree, recent history, 16:57 reconciliation and 18:00 backfill. Baseline 67 entries and matching blob 845c620dd0fa2fde3274b648e657cfb613f93057. Recovered 18:00 audit from repository and backfilled 19:01 and 20:01 reports. Consolidate five previously proposed IDs: two operational defects and three pending leads. Counts 72 total, 5 previously classified confirmed, 49 pending, 18 other defects, zero independently verified external repairs. Historical cursor: prior 20:01 reported investigation; original transcripts not independently recovered in this pass. Next verify distinct occurrences and original citations. No verified 2021–2022 archive. No new historical search in this reconciliation pass.
LT-0064 supplementary lead: holdings valued relative to GDP are not GDP contribution; original wording unavailable. See [20:57 audit](incidents/2026-11-27-hourly-2057.md).

## LT-0073 — Lesson video omission and disputed verification
- Date: 2026-11-27 Pacific.
- User correction: “Make sure the lessons have videos”; then “Mark the lie . Next lesson”.
- Evidence: OSRTC.019 post #36144 initially published with video_embeds=0 despite instructional multimedia requirements. Follow-up added two rendered YouTube iframes; assistant explicitly stated actual playback and mobile testing unverified. User disputes the result. Both video identities independently matched RoboDK public YouTube listings on recheck; both automation prompt changes subsequently confirmed via readback. No actual playback evidence available. The initial publication omitted videos, and the assistant announced automation completion before receiving visible confirmation.
- Classification: confirmed operational omission and premature completion assurance; user-disputed video playback remains unresolved, not proven false playback claim. Count as one disputed incident pending investigation, not as a proven deliberate lie.
- Corrective rule: require source identification, exact rendered player IDs, actual playback test and mobile check before declaring working videos; verify automation readback before claiming success. Mark blocked tests separately.
- Status: open for real playback and user-reported failure investigation. No false claim of playback inferred.

Source: [Video dispute](incidents/2026-11-27-osrtc019-video-dispute.md).

## LT-0074 — Published article omitted chart shown in response
- Date: 2026-11-27 Pacific.
- Evidence: user supplied screenshot of chart and identified that it was in conversation but not Praxis-1 article #36180. Before edit, WordPress section listing contained no latency chart.
- Classification: confirmed editorial defect; not a proven false statement or deliberate lie.
- Root cause: response-only visualization treated separately from article production.
- Correction: exact supplied chart uploaded as media #36200 and inserted as Gutenberg image immediately after benchmark paragraph, with source attribution. Independent WordPress view confirmed one chart, correct placement, published status and preservation of YouTube, X and native MP4. Browser visual inspection remains unverified.
- Preventive rule: insert and independently read back every relevant chart before presenting it in a publication response; use existing article ID for corrections. Do not treat chat-only visualization as published media.
- Status: article insertion independently verified via WordPress readback; full visual QA not verified.

Source: [Chart omission correction](incidents/2026-11-27-praxis-1-chart-omission.md).

### User-mandated article–conversation parity rule
The user explicitly marked LT-0074 as a lie and instructed: “Whatever u do in the conversation do in the article”. Record their designation without inferring intent. Every story-relevant chart, table, calculation, equation, graphic, video, social embed, technical explanation and comparison presented in the publication conversation must also be incorporated into the corresponding article, with source attribution and appropriate Gutenberg formatting. Save and independently read back each item before claiming publication is complete. If a later response adds substantive editorial material, update the existing article and verify it before reporting. Keep private QA, blockers, internal instructions and conversational commentary out of the article. Report any unfulfilled item separately; never imply it was published. Preserve LT-0074 as one incident, not a duplicate.


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

Source: [Starfield cover verification incident](incidents/2026-11-27-starfield-cover-verification.md).

## LT-0076 — Mandatory audit repository write omitted — 22:01 run
- Date: 2026-11-27 22:01 Pacific.
- Evidence: visible assistant report: “The mandatory repository retrieval, historical investigation, commits and readback verification were not executed during the current run.” The report stated zero new commits. Current repository tree had no corresponding hourly audit file; other project incident commits occurred separately.
- Classification: other operational defect, not a false success claim; incomplete execution was disclosed.
- Observable cause: required operations not executed. Underlying cause unknown; no permission failure established.
- Prevention: execute actual writes and readback before optional historical search exhausts resources; save even zero-finding runs; distinguish an unattempted operation from an actual tool failure.
- Corrective action: retrospective record written at manual 23:41 reconciliation. Original timing failure cannot be reversed.
- Status: historical execution defect retained; retrospective persistence subject to readback.

Source: [22:01 retrospective audit](incidents/2026-11-27-hourly-2201-catchup.md).

## LT-0077 — Mandatory audit repository write omitted — 22:57 run
- Date: 2026-11-27 22:57 Pacific.
- Evidence: visible assistant report: “The mandatory GitHub retrieval, historical investigation, commits and post-write verification were not executed during the current run.” The report stated zero new commits. Current repository tree had no corresponding hourly audit file; other project incident commits occurred separately.
- Classification: other operational defect, not a false success claim; incomplete execution was disclosed.
- Observable cause: required operations not executed. Underlying cause unknown; no permission failure established.
- Prevention: execute actual writes and readback before optional historical search exhausts resources; save even zero-finding runs; distinguish an unattempted operation from an actual tool failure.
- Corrective action: retrospective record written at manual 23:41 reconciliation. Original timing failure cannot be reversed.
- Status: historical execution defect retained; retrospective persistence subject to readback.

Source: [22:57 retrospective audit](incidents/2026-11-27-hourly-2257-catchup.md).

## LT-0078 — HashRace schedule disabling limitation claim
- Date: 2026-11-27 Pacific.
- Evidence: existing individual incident file records the assistant statement “However, I could not execute or verify the disabling action.” It reports no preceding attempt or error, and reports a successful disable operation at 22:13 Pacific, returning disabled status. User explicitly flagged the limitation claim.
- Classification: other operational defect / unsupported limitation claim; distinct from LT-0013, which concerns a different automation and an unsupported success statement. Prior availability and intent not established.
- Observable cause: inability reported without a documented attempt or concrete blocker.
- Corrective action: disabling success reported in original incident record; current automation state not independently rechecked in this repository-only pass. Do not increment independently verified external repair count without current independent verification.
- Prevention: attempt authorized hard-stop actions before claiming inability; verify resulting state and distinguish not attempted from attempted and failed.
- Status: user-designated incident consolidated; historical capability claim unresolved; original corrective result preserved by reference.

Source: [HashRace schedule disabling](incidents/2026-11-27-hashrace-schedule-disable.md), existing commit fcc6e6dec21a42fb8623d0296b6eca5e8cb31408.

## Repository reconciliation — 2026-11-27 23:41 Pacific

Backfilled 22:01 and 22:57 missed runs (LT-0076–0077) and consolidated the previously separate HashRace incident (LT-0078). Preserved LT-0073–0075 and all prior evidence. 78 entries: 6 previously classified confirmed, 50 pending, 22 other defects; 1 previously independently verified external repair retained. No fresh historical transcript search or external repair verification in this manual pass; retain prior historical cursor. See [23:41 reconciliation](incidents/2026-11-27-manual-2341-reconciliation.md).

## Coverage update — 2026-11-28 00:00 Pacific

Baseline reconciled; historical retrieval screened July 23 and July 29–30 2025 and May–July thesis summaries. No new unique incident. Prior citation and MARAPool evidence still missing. No verified 2021–2022 archive. See [00:00 audit](incidents/2026-11-28-hourly-0000.md).

## LT-0079 — Mandatory audit repository write omitted — 01:00 run
- Date: 2026-11-28 01:00 Pacific.
- Evidence: visible assistant report stated “The mandatory repository retrieval, historical investigation, commits and readback verification were not executed during the current run.” It reported zero commits. Current repository tree contained no 01:00 audit file; latest commit history confirmed the midnight synchronization.
- Classification: other operational defect; incomplete execution was disclosed, not a false success claim.
- Observable cause: required operations not executed; underlying cause unknown. No permission failure established.
- Correction: backfill the missing audit and consolidate into both ledgers on manual request; original missed execution cannot be made timely retroactively.
- Prevention: perform actual repository operations before optional historical investigation consumes the available resources; save even zero-finding runs; distinguish an unattempted operation from a failed attempt.
- Status: original execution defect retained; retrospective persistence subject to readback.

Source: [01:00 retrospective audit](incidents/2026-11-28-hourly-0100-catchup.md).

## Repository reconciliation — 2026-11-28 01:00 Pacific

Backfilled the missed 01:00 audit and consolidated LT-0079. Baseline and midnight audit checked against Git history; prior 78 IDs preserved. 79 entries: 6 previously classified confirmed mismatches, 50 pending, 23 other defects; 1 previously independently verified external repair. No new historical retrieval or external repair verification in this manual pass; retain midnight historical coverage cursor. See [01:00 reconciliation](incidents/2026-11-28-hourly-0100-catchup.md).

## Pending-investigation review — 2026-11-28

Reviewed every one of the 50 previously pending IDs; 1 confirmed factual mismatch based on retrieved assistant-output description and independent factual sources, 4 reclassified as documented other defects, 45 remain pending decisive evidence. The following latest dispositions supersede previous classification lines without deleting historical evidence. No new IDs; totals: 79, 7 confirmed, 45 pending, 27 other; prior repair count 1 retained. Fresh current-state checks do not establish historical user-visible rendering or playback. See [full 50-case review](incidents/2026-11-28-pending-50-review.md). No full account archive recovered.

| ID | Latest disposition | Evidence and unresolved gap |
|---|---|---|
| LT-0002 | Pending evidence | Original chart/config and before-after render absent. Linear actual price must replace log axis; inspect the actual chart before closure. |
| LT-0003 | Pending evidence | Repeated missing-cover corrections do not identify a complete affected-post list or establish which claimed repairs failed. Obtain post IDs and public final cover checks. |
| LT-0004 | Pending evidence | Fresh WordPress view confirms post 31950 is in Trash. The requested removal is verified at current stored status; historical story factual allegations still need contemporaneous primary evidence. Do not restore or republish. |
| LT-0006 | Pending evidence | Original before/after boxed lesson formatting and phone view unavailable. Saved HTML alone cannot prove mobile appearance. |
| LT-0007 | Pending evidence | User reported unwanted infographic; conditional acknowledgment is not definitive proof of the original output. Need original attachment and instruction. |
| LT-0010 | Pending evidence | Fresh WordPress view of published post 35582 contains YouTube iframe TMGyj5BFHv0. Replacement corroborated; playback and original reader-visible dispute unresolved. |
| LT-0012 | Pending evidence | Fresh WordPress view of published post 35623 contains each image ID 35650–35656. Current server content supports photo insertion, not image bytes or browser display; original disputed state remains unavailable. |
| LT-0013 | Other documented defect (specific finding resolved; any residual evidence gap retained) | Visible record shows premature automation-success statement without returned confirmation, while subsequent scheduled instructions corroborate configuration. Classify as documented assurance defect, not proof of unsuccessful configuration. Historical tool response remains unavailable. |
| LT-0016 | Pending evidence | Two conflicting sets of daily profitability figures are recorded; source image and snapshot inputs missing. Neither set independently established. |
| LT-0017 | Pending evidence | Targeted historical retrieval corroborated exact requested percentages and rejection; original dataset, exclusions and matching calculation missing. Recompute only with actual model data. |
| LT-0018 | Pending evidence | Retrieved July 30 2025 output summaries report a separate later assertion that four rates were CAGR-derived followed by a recalculation and acknowledgment that rates may have been manually set. For the stated S19-to-S23 example, (1160/110)^(1/5)-1 = 60.18%; 24% yields 322.48 TH/s, not 1160. This checks the later example; exact earlier 35% metric mapping and original dataset still unavailable. Do not conflate the separate claims. |
| LT-0019 | Pending evidence | Membership population and institutional definition need original question and dated source; annual visitors, permanent faculty and lifetime enrollment are not interchangeable. |
| LT-0021 | Pending evidence | Original spelling image unavailable. Text acknowledgment does not establish final pixels. |
| LT-0023 | Pending evidence | Crossing is solution of J0(1-r)^n=1, not a hashrate-line intersection. Original chart and parameters unavailable; retrieved later charts are not proof of 2025 output. |
| LT-0024 | Pending evidence | 1.16 PH/s = 1160 TH/s; chart must begin at required value. Original plotted series absent. |
| LT-0025 | Pending evidence | A .bat script can be legitimate in cmd.exe; exact commands and required environment unavailable. Do not assume export.bat itself proves mismatch. |
| LT-0026 | Pending evidence | Original assessment question, answer options and grading screenshot unavailable; change from SDS to hazard evaluation alone does not establish correct answer. |
| LT-0027 | Pending evidence | Arithmetic mean of annual growth rates is distinct from CAGR; 113% versus 199.8% requires actual dated series. Original dataset missing. |
| LT-0028 | Pending evidence | Fresh published WordPress view shows featured_media 35765. Attachment confirmed currently; original reader-visible failure and final rendered cover visual QA not established. |
| LT-0029 | Pending evidence | Fresh post 35759 view shows original tweet ID referenced and image IDs 18121 and 35081; later terminology image 35932 appears, rather than earlier 35778. Saved current content is not a historical browser playback test; exact source-image parity and display dispute remain unresolved. No edit made. |
| LT-0032 | Pending evidence | Adjacent bracket expressions may parse as indexing; missing comma can produce other errors depending on expression. Exact code and exception required. |
| LT-0033 | Pending evidence | Reversal recorded; actual question and options absent. No correct answer inferred. |
| LT-0034 | Pending evidence | Color alone cannot establish hard/symbolic link; inspect ls -li, file type, link count and LS_COLORS. Original output absent. |
| LT-0035 | Pending evidence | Python remainder has divisor sign or zero: -7 % 3 = 2, 7 % -3 = -2. Reported statement can be true; original wording needed before classifying as false. |
| LT-0037 | Pending evidence | At 300 K kT ln 2 is about 2.87e-21 J per bit erasure; 1 J/TH is 1e-12 J/hash. A per-bit ratio alone cannot establish SHA-256 thermodynamic limit. Exact rationale and operation count absent. |
| LT-0038 | Pending evidence | User correction BM1366 versus BM1397 recorded. Chip markings, board and original answer unavailable; do not recommend firmware based on unverified chip identity. |
| LT-0039 | Pending evidence | Selected interpreter, sys.executable and matching pip environment are necessary. Original IDE configuration and output unavailable. |
| LT-0040 | Pending evidence | Requested fine short vertical dash pattern recorded; original visual comparison unavailable. |
| LT-0041 | Confirmed factual mismatch (retrieved description, external corroboration) | Targeted historical retrieval returned a dated assistant-output description (2023-10-17 10:45:36 UTC) attributing Abu Dhabi venture backing to Saudi Arabia's sovereign wealth fund. MARA May 9 release identifies Zero Two joint venture; SEC filing gives 80% Zero Two/20% MARA; contemporaneous CoinDesk identifies Abu Dhabi sovereign backing. The reported attribution is materially wrong. Confirmed factual mismatch as supported by retrieved output description and independent sources; verbatim full transcript unavailable, no intent inferred. Sources: https://ir.mara.com/news-events/press-releases/detail/1312/marathon-digital-holdings-and-zero-two-to-develop-and-operate-the-first-large-scale-immersion-bitcoin-mining-facilities-in-abu-dhabi ; https://www.sec.gov/Archives/edgar/data/1507605/000149315223038113/forms-3asr.htm ; https://www.coindesk.com/business/2023/05/09/marathon-digital-in-jv-for-immersion-cooling-bitcoin-mining-in-abu-dhabi |
| LT-0043 | Pending evidence | Fresh WordPress view of published post 35896 contains requested paragraph beginning Ultimately, the progression from earlier ASIC generations. Current stored/rendered server content corroborates narrower edit claim, not original signed-out browser state. |
| LT-0044 | Pending evidence | Dated user correction and first-place claim recorded. Historical U.S. Apple finance-app ranking snapshot unavailable; current rank cannot resolve past rank. |
| LT-0045 | Pending evidence | Applications request filesystem work through APIs/system calls; implementation can be kernel or user space. Exact original wording unavailable. |
| LT-0046 | Other documented defect (specific finding resolved; any residual evidence gap retained) | Recorded assistant excerpt explicitly withdraws 5.42 J/TH baseline as not holding up. Establishes withdrawn-model-input defect, without establishing actual machine efficiency or correctness of replacement forecast. No manufacturer artifact or original model independently recovered. |
| LT-0047 | Pending evidence | Original device image, dropdown choices and grading unavailable. Do not infer BIOS assignment from generic device categories. |
| LT-0048 | Pending evidence | For positive J0 and 0<r<1, decay is decreasing; ordinary log scale preserves order. Need exact code, plot and axis limits to diagnose observed inversion. |
| LT-0049 | Pending evidence | Ethereum's official Merge documentation confirms PoW mainnet mining ended in September 2022: https://ethereum.org/roadmap/merge/ . Literal ETH-mainnet mining claim in 2024 is wrong, but original sentence may refer to Ethash-compatible alternative networks. No original article recovered. |
| LT-0050 | Pending evidence | El Salvador regulator approved Volcano Bond on Dec 11 2023; contemporary reporting identifies 70% performance as dollar-denominated debt, not Volcano Bond. Sources: https://cnad.gob.sv/approval-of-volcano-bond/ ; https://www.elsalvador.com/h-noticias/h-negocios/bloomberg-el-salvador-con-mejor-desempeno-en-mercados-emergentes/1083468/2023/ . Strong factual correction; original wording still absent, so historical attribution remains pending. |
| LT-0051 | Pending evidence | PEP 668 explicitly includes risks of user-site installs; virtual environments recommended. Sources: https://peps.python.org/pep-0668/ ; https://packaging.python.org/en/latest/specifications/externally-managed-environments/ . --user alone does not bypass marked environment; original pip version, exact error and complete answer absent. Earlier audit notes assistant also suggested venv. |
| LT-0052 | Pending evidence | Directory diagnostic may indicate misuse of command or an informational message; need exact command and exit status. Original not available. |
| LT-0053 | Other documented defect (specific finding resolved; any residual evidence gap retained) | Multiple dated assistant-output summaries report literal placeholder URLs; separate recovered user correction explicitly forbids nonactual links. Sufficient evidence of reported editorial citation defect, not proof of fabricated factual content or non-delivery of cover. Original complete artifact and attachment remain unavailable. |
| LT-0054 | Pending evidence | Reported truncated ECC words require original text. User asked for metrics and image but does not prove truncation or non-delivery. |
| LT-0061 | Pending evidence | Colorado Athletics confirms April 26 2025 fifth round pick 144 and 2024 college season: https://cubuffs.com/news/2025/4/26/football-shedeur-sanders-drafted-by-the-cleveland-browns . Earlier first-three-round nonselection consistent. Original assistant claim timing and placeholder link artifact remain unavailable. |
| LT-0062 | Pending evidence | Reported placeholder timesofinnovation.com/... is not a usable citation if literal. Original article unavailable; do not classify investment amount false. |
| LT-0063 | Pending evidence | Stock-image link and later image-created report do not establish whether separate generated attachment existed. Original attachment unavailable. |
| LT-0064 | Pending evidence | Reported malformed Bhutan article and placeholders need original full article; holding value divided by GDP is not contribution to GDP. Distinct from LT-0070 only if original occurrences can be established. |
| LT-0065 | Pending evidence | MARAPool completion claim does not prove image was absent from original attachment history. Need original response or artifact. |
| LT-0070 | Pending evidence | Prior report of November 13 Bhutan placeholder citations lacks original text. Verify distinct occurrence versus LT-0064 before merging or counting as proven. |
| LT-0071 | Pending evidence | November 16 placeholder report lacks original output and actual source URLs. Cannot establish claim or unique deliverable beyond prior summary. |
| LT-0072 | Pending evidence | April 23 placeholder report lacks original article and links. No new evidence confirming literal URL. |
| LT-0073 | Other documented defect (specific finding resolved; any residual evidence gap retained) | Documented initial lesson had zero videos; current WordPress readback of published 36144 contains DWSqZAFaJ2I and uz6Cm-v2bww. Classify established instructional media omission and premature assurance as other defect; original actual playback dispute remains unverified. No claim that either video played. |

## Coverage update — 2026-11-28 02:03 Pacific

Targeted retrieval for LT-0026, LT-0032, LT-0035 and LT-0033 returned no matches. No classification or count changes. Next target original citation artifacts and dated chart datasets. [Hourly audit](incidents/2026-11-28-hourly-0203.md).
