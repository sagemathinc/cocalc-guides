# Reviewing Agent Commits in CoCalc-AI

A short illustrated guide to using CoCalc-AI's git review drawer as the careful
second phase after fast agent work.

Audience: software engineers, project maintainers, and researchers who use Codex
for real repository changes but want a workflow that remains auditable.

The guide emphasizes:

- small commits as review units
- commit-by-commit coverage with reviewed state
- private review notes
- inline diff comments tied to file, side, line, hunk, and snippet
- sending actionable review comments back to Codex with exact diff context
- large-diff navigation through search, context controls, changed-file jumps,
  and virtualized rendering
- import/export of review state
