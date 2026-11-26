# Beyond Softwar featured cover audit

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
