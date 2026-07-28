# Security And Verification

## Credentials

Accept an ElevenLabs key only from the process environment or a protected local
`.env` file. Never ask a user to paste it into chat, a command argument, a
public file, a commit, shell history, or logs. Never display its value, length,
prefix, suffix, or a masked substitute.

Before a credential file is created or changed, obtain explicit approval. Check
that `.env` is ignored by Git before the user writes it. The user should write
the secret using a local editor or terminal; the agent does not read its
contents. Reject a symlink or non-regular file. Set and verify restrictive file
permissions using platform-appropriate tools.

## Paid Or External Actions

Before every first media upload, identify the exact filename, provider,
purpose, and potential quota or cost. Wait for a clear approval for that upload.
Do not substitute local transcription when hosted transcription is declined;
explain the lower-confidence alternative and wait for explicit selection.

For voice cloning, require the user to confirm they are the speaker or have
explicit permission to clone that speaker. Name the source sample and provider
before upload. Do not fall back to an impersonating voice or a generic voice
without a new user decision.

## Local Evidence

Do not claim readiness based on an intended command. Report only completed,
locally observable checks. A setup check must not upload media, query account
usage, create a project, edit footage, or render output.
