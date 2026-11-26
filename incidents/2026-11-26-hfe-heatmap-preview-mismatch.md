# LT-0015 — HFE heatmap preview differed from published chart

Date: 2026-11-26. WordPress post #35717, original media #35710. User reported “the rendition u put in the conversation looks totally different from the one in the actual post.... thats a lie” and supplied two screenshots.

## Evidence and finding
The conversation displayed a polished nine-model SVG matrix; uploaded chart used scatter markers for 18 models with missing category/model labels, large whitespace and clipped/low-contrast numerals. The screenshots show the discrepancy directly. Prior answer disclosed that independent chart inspection remained outstanding, but nevertheless called the chart mathematically appropriate and published it without visual parity. Confirmed misleading preview-to-publication mismatch, not evidence of deliberate intent or fabricated upload.

## Cause and corrective action
Observable mechanism: separate renderers produced different visual artifacts; upload and API readback were treated as enough to ship. Generated a real 18x4 rectangular matrix preserving all 72 values from previous chart data, with model names, category labels, centered percentages and fixed color bins. Rejected an initial overflowing render after inspecting it. Final uploaded PNG media #35727, 1200x1350, visually inspected from the exact bytes submitted. Replaced the original image block in existing article, not a new post. WordPress view readback: {"status":"publish","corrected":true,"old":false,"featured":35713,"qr":true,"social":true}.

## Prevention
Use a single final image asset for public post and conversation preview, or link to that exact asset rather than drawing an independent mockup. Inspect actual output before publication, checking all labels, row/column completeness, numerical content, clipping, contrast, responsive readability. Do not report independent browser verification from API markup. Reject malformed renderers before publishing. Preserve source data and original article identity.

## Remaining limitations
Direct public CDN/browser retrieval unavailable (container DNS failed); exact submitted bytes inspected and WordPress readback confirmed replacement, but public browser appearance not independently established. Primary PDF could not be reopened (fetch size limit); this correction preserves existing values, not a fresh source validation. Font differs from earlier preview. No intent inferred.
