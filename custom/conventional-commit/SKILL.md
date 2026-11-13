---
name: conventional-commit
description: Writes commit messages in English following Conventional Commits. Use when the user asks for a commit message or wants to commit staged changes.
---

Write a commit message for the staged changes.

1. Run `git diff --staged` to see what is actually being committed. If nothing is staged, say so and stop.
2. Pick the type: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `build`, `ci` or `chore`.
3. Add a scope in parentheses only when it clarifies the change, for example `feat(auth): ...`.
4. Write the subject in English, in the imperative mood ("add", not "added" or "adds"), lowercase, no trailing period, 72 characters maximum.
5. Add a body only when the reason for the change is not obvious from the subject. Explain why, not what.
6. If the diff mixes unrelated changes, tell the user to split it into several commits and propose how, instead of writing one vague message.
7. Show the message and ask for confirmation before running `git commit`. Never push.
