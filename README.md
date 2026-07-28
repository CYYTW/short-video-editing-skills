# Safe Short Video Skills

Reusable, consent-gated Skills for AI-assisted vertical video editing.

## Install for Codex

```powershell
npx skills add OWNER/short-video-editing-skills --skill safe-video-editing-setup -a codex
npx skills add OWNER/short-video-editing-skills --skill safe-short-video-editor -a codex
```

Replace `OWNER` with the GitHub account shown in this repository URL.

## Included Skills

- `safe-video-editing-setup`: inspect and prepare a local video-editing environment without creative work or paid API calls.
- `safe-short-video-editor`: edit supplied media into an evidence-backed vertical short with explicit consent, preview QA, and final-file QA.

## Security Boundary

This repository intentionally contains no credentials, source media, fonts, voice samples, or generated videos. Each user supplies their own tools, media, permissions, and API credentials locally.
