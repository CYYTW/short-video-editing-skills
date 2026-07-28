# Output Contract

Keep generated artifacts beside the source media:

```text
edit/
  project.md
  transcripts/<source>.json
  corrected-transcript.md
  edl.json
  master.srt
  clips/
  animations/slot_<id>/
  qa/
  preview.mp4
  final.mp4
```

`project.md` records source identifiers, approved strategy, significant
decisions, unresolved questions, and each render/QA attempt. `qa/` retains
boundary checks, first/last/mid samples, subtitle-safe-area checks, stream
inspection, and full-decode evidence. Retain only one formal final outwardly.
