---
name: safe-short-video-editor
description: Create a verified vertical Reel, Short, TikTok, vlog, or talking-head video from user-provided media with source inspection, consent-gated transcription, word-aligned cuts, Traditional Chinese subtitles, preview QA, and final delivery. Use when a user asks to transcribe, cut, subtitle, preview, or export a short-form video.
---

# Safe Short Video Editor

Create a real, evidence-backed vertical short from supplied media. Read
[eight-step workflow](references/eight-step-workflow.md), [production
rules](references/production-rules.md), and [output contract](references/output-contract.md)
before changing media.

## Non-Negotiable Rules

1. Do not overwrite, move, rename, or delete the source media. Keep every new
   artifact under an adjacent `edit/` directory.
2. Inspect each source with `ffprobe` before creating the work directory.
3. Before first upload of a source file, identify the filename, say that it
   will be uploaded to the named transcription provider, explain its purpose
   and potential cost, then wait for explicit approval.
4. Cache word-level, verbatim transcripts by unchanged source. Never silently
   replace unavailable cloud transcription with a lower-confidence local path.
5. After content analysis, describe the proposed edit in plain language and
   wait for approval before choosing edit points or adding B-roll, animation,
   music, sound effects, CTA, colour styling, or publishing actions.
6. Snap edit edges to complete-word boundaries and keep 30-200 ms of natural
   padding. Extract, process, and verify retained segments independently, with
   approximately 30 ms audio fades at boundaries.
7. Generate output-timeline subtitles and apply them last, after every overlay
   and card. Use a verified Traditional Chinese font; do not substitute one
   silently.
8. Render a complete 720p preview and inspect the rendered file. Render a
   1080x1920 formal final only after the user explicitly approves that preview.

## Completion

Report only verified work. State the source evidence, upload consent state,
transcript cache state, approved strategy, preview path and QA, final path and
final-file QA, retained artifacts, repair-pass count, and unresolved issues.
