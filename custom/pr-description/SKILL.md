---
name: pr-description
description: Writes a Pull Request title and description in English from the branch changes. Use when the user is about to open a PR or asks for a PR description.
---

Write a Pull Request description for the current branch.

1. Compare the branch with its base using `git log` and `git diff <base>...HEAD`. Ask which branch is the base if it is unclear.
2. Title: short, in English, imperative mood, following Conventional Commits style (for example `feat(parser): support nested blocks`). It becomes the squash commit message, so make it a good one.
3. Description with exactly these sections:
   - **Summary**: what the PR does and why, in one or two sentences.
   - **Changes**: a bullet list of the concrete changes, one line each, with file paths or names in backticks.
   - **Notes**: anything the reviewer should know (limitations, things not tested, follow-ups). Omit the section if there is nothing to say.
4. Link related issues with `Closes #n` only if the user mentions them. Never invent issue numbers.
5. Keep it short. Describe what the diff really does, not what it was meant to do.
