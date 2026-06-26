# Contributing to tyohame-tietojohtaminen

Thanks for working on **tyohame-tietojohtaminen**. This guide keeps the repository consistent and reviewable.

## Workflow

1. Branch off the default branch. Never commit directly to it.
2. Use a descriptive branch name: `feat/...`, `fix/...`, `chore/...`, `docs/...`.
3. Keep changes small and independently testable.
4. Open a pull request and fill in the template. CI (where configured) must be green.

## Commit messages

Use [Conventional Commits](https://www.conventionalcommits.org/): `type(scope): summary`.
Common types: `feat`, `fix`, `chore`, `docs`, `refactor`, `test`, `ci`.
Write commit subjects in English, imperative mood.

## Before you push

- Code builds / typechecks locally.
- Tests pass; new behavior is covered by a test.
- No secrets committed. Real values live only in a local, git-ignored `.env`;
  add new variables to `.env.example` as empty placeholders.
- Update `CHANGELOG.md` under `[Unreleased]` for any user-visible change.

## Code style

- Follow the existing patterns in the codebase.
- `.editorconfig` defines whitespace; respect it.
- Prefer clear names and small functions over comments that restate the code.
