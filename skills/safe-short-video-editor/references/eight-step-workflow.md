# Eight-Step Workflow

1. **Inventory**: use `ffprobe` to record video and audio streams, duration,
   orientation, dimensions, frame rate, rotation, sample rate, colour tags,
   and full decode status. Confirm the source and 9:16 target.
2. **Transcribe**: after exact upload approval, create or reuse a cached,
   word-level verbatim transcript. Flag uncertain names, dates, numbers, and
   proper nouns instead of guessing.
3. **Organize**: prepare a readable corrected transcript and identify hook,
   narrative, repetition, failures, dead air, unfulfilled promises, likely
   runtime, and visual ambiguities. This is analysis, not an edit decision.
4. **Propose**: explain the viewer outcome, opening line, narrative spine,
   chosen and removed material, reordering, estimated length, visual direction,
   captions, and any proposed cards, B-roll, animation, music, effects, or CTA.
   Wait for approval.
5. **Rough cut**: build `edl.json` from word-aligned ranges. Record source,
   start, end, beat, quote, reason, and consistent output offsets for every
   retained range.
6. **Finish visuals**: apply only approved colour treatment, cards, B-roll, and
   animation. Generate subtitles from output-timeline timestamps and burn them
   last, inside the platform safe area.
7. **Preview and QA**: create one complete 720p preview. Inspect every cut
   boundary at approximately plus/minus 1.5 seconds, first/last/mid samples,
   subtitle safety, streams, duration, colour, mix, sync, and full decode.
   Self-correct only evidence-backed defects, with at most three passes.
8. **Final delivery**: after explicit preview approval, render `final.mp4` at
   1080x1920. Re-inspect the final file itself at all boundaries and samples,
   perform a full decode, and deliver only after all checks pass.
