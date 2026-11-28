# Drew Mestemaker embed audit

## LT-0080 — Unrequested interview substituted for Drew Mestemaker highlights
- Date: 2026-11-28. WordPress post 36425.
- Evidence: user provided X status 2126595844858425554, then corrected the assistant: “The video needs to be a highlight of Drew” and “Use the emebed o sent u. From x”.
- Classification: Other documented editorial/instruction-following defect, not a separate false factual claim.
- Action: removed the YouTube interview; retained the same user-supplied X status.
- Prevention: match media to user-provided source and requested footage; never substitute unrelated interviews.
- Status: interview removal verified by post readback; playback of requested footage not independently tested.

## LT-0081 — Embed correction reported while rendered article showed only a link
- Date: 2026-11-28. WordPress post 36425.
- Evidence: assistant said “Updated the published article” and “Verified the saved WordPress embed”; it explicitly acknowledged actual video playback unverified. User then requested repeated repair. WordPress context=view returned only an anchor in the embed wrapper, not embedded post markup.
- Classification: confirmed completion mismatch at functional embed level, not a claim that playback was verified.
- Root cause: verified saved Gutenberg block rather than provider output; x.com canonical URL returned link-only fallback in WordPress.
- Action: use twitter.com URL for the identical status ID with native Gutenberg provider. Fresh context=view returned embed-x, twitter-tweet blockquote containing original post text and platform.x.com/widgets.js. No save warnings.
- Prevention: retrieve rendered HTML, reject link-only fallbacks, verify same status ID, then separately test browser rendering and video playback before calling functional QA complete.
- Status: server-rendered embed markup repaired and verified; mobile browser rendering and actual video playback remain unverified. Public screenshot endpoint reported ready but image not independently inspected.
