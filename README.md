# Safe Short Video Skills

Reusable, consent-gated Skills for AI-assisted vertical video editing.

## Install for Codex

```powershell
npx skills add CYYTW/short-video-editing-skills --skill safe-video-editing-setup -a codex
npx skills add CYYTW/short-video-editing-skills --skill safe-short-video-editor -a codex
```

To install both skills interactively, use:

```powershell
npx skills add CYYTW/short-video-editing-skills
```

## Included Skills

- `safe-video-editing-setup`: inspect and prepare a local video-editing environment without creative work or paid API calls.
- `safe-short-video-editor`: edit supplied media into an evidence-backed vertical short with explicit consent, preview QA, and final-file QA.

## Security Boundary

This repository intentionally contains no credentials, source media, fonts, voice samples, or generated videos. Each user supplies their own tools, media, permissions, and API credentials locally.
