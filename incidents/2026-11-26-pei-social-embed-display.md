# PEI social embed display audit

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
