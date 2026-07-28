---
name: safe-video-editing-setup
description: Safely inspect, install, repair, or verify a local AI short-video editing environment including video-use, FFmpeg, subtitle fonts, and ElevenLabs credentials. Use when a user asks to set up, connect, repair, or verify their video-editing tooling. Do not use to transcribe, edit, preview, or render media.
---

# Safe Video Editing Setup

Prepare or repair the environment without starting creative work. Produce an
evidence-backed readiness report, never a transcript, upload, edit, preview,
or render.

Read [setup runbook](references/setup-runbook.md) and [security and
verification](references/security-and-verification.md) before making changes.

## Rules

1. Inspect before changing anything. Check the OS, architecture, active agent,
   Git, Python, `uv`, FFmpeg, `ffprobe`, subtitle fonts, Skills directory, and
   applicable repositories.
2. Treat a missing, invalid, dirty, or unexpected-origin repository as a hard
   stop. Never rewrite remotes, reset, pull, clone over it, install packages,
   or register Skills until the user chooses a safe remedy.
3. State every mutation and its location before cloning, installing packages,
   downloading fonts, creating symlinks, changing Skills directories, or
   changing credential storage. Wait for explicit approval.
4. Treat HyperFrames as optional. Check or install it only when the user
   explicitly requests HTML, CSS, or GSAP animation work.
5. Never reveal, copy into a command, log, commit, or infer a credential.
   Verify only that an approved credential source exists.
6. Use local, no-cost checks for readiness. Do not upload media, call
   transcription, inspect cloud quota, create an edit directory, or render
   video during setup.

## Completion

Report observed paths, exact repository state, tool evidence, font evidence,
approved changes performed, and every remaining blocker. Do not call the
environment ready unless all required local checks pass.
