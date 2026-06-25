# Security Policy

## Reporting a vulnerability

**Do not open a public issue for security or data-handling concerns.**

Report privately to **oskari.vatanen94@gmail.com**. Include:

- a description of the issue and its impact,
- steps to reproduce (proof of concept if available),
- affected version / commit.

You can expect an acknowledgement within a few business days. Please give a
reasonable window to remediate before any public disclosure.

## Supported versions

This is an actively developed project; only the latest default-branch state is
supported. Fixes land on the default branch.

## Handling secrets

- Secrets (API keys, tokens, credentials) are configured via environment
  variables and are **never** committed.
- `.env` is git-ignored. `.env.example` documents required variables with
  empty placeholder values only.
- If you discover a committed secret, treat it as compromised: rotate it and
  report via the channel above.
