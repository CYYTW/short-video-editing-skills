# Production Rules

## Audio And Cuts

- Keep voice intelligible and natural.
- Never cut inside a word or remove word heads and tails.
- Preserve 30-200 ms of natural padding outside spoken boundaries.
- Use around 30 ms audio fade-in and fade-out at each retained segment edge.
- Do not add music or effects without explicit creative approval.

## Visuals And Captions

- Use B-roll as purposeful sustained coverage, not rapid back-and-forth filler.
- Apply technical colour correction only when needed or approved; do not call
  unrequested styling a necessary correction.
- Keep editable animation sources with their rendered output.
- Use output time for subtitle timestamps: `word.start - segment_start +
  segment_offset`.
- Keep captions to readable one- or two-line chunks and avoid faces and
  platform UI safe areas.

## QA

- Check the rendered preview, not merely the timeline or source clips.
- Inspect flash frames, jumps, pops, subtitle hiding, overlay timing, sync,
  colour, and mix at each boundary.
- Verify video and audio streams, duration, dimensions, and full decode for
  preview and final separately.
- Never call a preview a final, and never call a planned or partially rendered
  file complete.
