# LieTracker — Master Ledger

Last consolidated: 2026-11-26. Canonical cumulative incident record; preserve every stable incident ID and supporting evidence. Historical summaries are not full transcripts; no intent to deceive is inferred. Counts describe recorded entries only, not all conversations.

## Cumulative totals

| Category | Count |
|---|---:|
| All recorded entries | 49 |
| Confirmed claim/completion mismatches (as classified in source audits) | 5 |
| Pending investigations | 36 |
| Other technical/editorial defects | 8 |
| Independently verified external repairs | 0 |
| Unresolved or not independently verified | 49 |

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
