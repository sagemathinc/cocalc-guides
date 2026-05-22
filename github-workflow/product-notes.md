# Product Notes From Drafting This Guide

These notes are not part of the public guide. They capture product ideas that
became sharper while writing the GitHub workflow guide.

## Strong Ideas

### GitHub-ready project action

The guide wants a first-class setup action:

- install `gh` if missing
- run `gh auth status`
- explain how authentication is scoped
- verify that `git` and `gh` agree about the current repository

This could be a small project command or a Codex prompt template.

### Credential visibility and safety

Realtime collaboration makes GitHub integration powerful, but authentication
needs clear affordances. CoCalc-AI should make it obvious when a project has an
active GitHub credential and should explain the trust boundary for shared
projects.

### PR-from-agent receipt

When Codex opens a pull request, the product could show a compact receipt:

- branch name
- commits pushed
- tests or checks run
- PR URL
- review comments still unresolved

This would make agent-authored GitHub work easier to audit from the CoCalc side.

### Issue-to-workspace flow

A useful action would be:

> Open this GitHub issue as a CoCalc task.

That could create a branch, start a Codex thread with the issue body, and keep
the issue, terminal, code diff, and PR linked together.

## Smaller Ideas

### Shared terminal history as GitHub context

Codex can already use terminal history, but GitHub workflows make this especially
valuable: `gh pr checks`, failed CI logs, and release upload commands are all
high-signal context.

### Release checklist template

For repositories that publish artifacts, CoCalc-AI could provide a lightweight
release checklist: version, tag, changelog, build, checksum, upload, smoke test.

### GitHub auth reminder in teaching projects

For class or workshop projects, the UI could gently warn against authenticating
with a powerful personal GitHub account in a project that has many collaborators.
