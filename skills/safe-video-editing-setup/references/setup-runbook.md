# Setup Runbook

## Inspect First

Check the operating system, CPU architecture, active agent, Git, Python, `uv`,
`ffmpeg`, and `ffprobe`. Check Node.js, npm, npx, Bun, and HyperFrames only if
the user explicitly requests HyperFrames.

For each applicable existing repository, use `git -C <repo> rev-parse
--is-inside-work-tree` rather than testing whether `.git` is a directory. A
linked worktree uses a `.git` file. Capture the exact origin, branch or
detached state, commit, and `git status --short`.

Default expected origins:

```text
video-use: https://github.com/browser-use/video-use.git
HyperFrames: https://github.com/heygen-com/hyperframes.git
```

If an existing repository is not a valid worktree, has no origin, has an
unexpected origin, has no valid HEAD, or has a non-empty short status, stop.
Do not pull, reset, overwrite, reclone, install dependencies, or alter the
remote.

## Changes Need Approval

Before any mutation, list the exact action, location, and reason. This includes
cloning, package installation, downloading a font, large downloads, symlink
creation, Skill registration, and credential-file changes. Repeat the
repository inspection immediately before dependency installation or Skill
registration because its state may have changed.

## Subtitle Font

Use Source Han Sans TW for Traditional Chinese burned subtitles when available.
On macOS inspect `~/Library/Fonts`; on Linux inspect
`~/.local/share/fonts`. Require `SourceHanSansTW-Regular.otf` and
`SourceHanSansTW-Bold.otf` to be regular non-symlink files. When `fc-list` is
available, confirm it can list the family. Do not substitute a font silently.

If a font download is approved, use only the official Adobe Source Han Sans
release branch. Verify each downloaded OTF is a regular non-symlink file and
starts with `OTTO` magic bytes before declaring success.

## Optional HyperFrames

Use HyperFrames only when the approved creative strategy needs HTML, CSS, or
GSAP animation. Require Node.js major version 22 or newer. Do not change the
system Node.js version automatically. Read the checked-out upstream README,
CONTRIBUTING guide, package metadata, and lockfile before choosing an install
command.

## Ready Report

Report stable paths, repository origins and cleanliness, tool versions or
paths, font checks, precise Skill target, and credential-source presence. Do
not perform a paid cloud call merely to prove a key works.
