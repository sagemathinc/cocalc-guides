# Product Notes From Drafting This Guide

These notes are not part of the public guide. They capture product ideas that
became sharper while writing the software-install guide.

## Strong Ideas

### Install intent for Codex

The guide wants a first-class agent action:

- `Install the missing software for this error`
- `Make this notebook cell work`
- `Install this command and verify it`
- `Write setup notes for what changed`

The user should not have to know whether the answer is `apt-get`, `pip`,
`npm`, TeX Live, or a system library.

### Environment change receipt

After an install, CoCalc-AI could show a compact receipt:

- commands run
- packages installed
- files changed
- verification command
- snapshot id before install, when available

This would make agent-driven environment changes easier to trust.

### Snapshot affordance before risky installs

For installs that touch the root filesystem, add a lightweight prompt:

> Snapshot first?

This does not need to be scary. It should feel like a fast checkpoint, not a
formal backup workflow.

### Project setup file

Codex should be encouraged to maintain a project-local setup file such as:

- `SETUP.md`
- `setup.sh`
- `environment.yml`
- `requirements.txt`

The guide says “write down what changed” because reproducibility is the real
product outcome.

## Smaller Ideas

### Command-not-found helper

When a terminal sees `command not found`, the UI could offer:

- ask Codex to install it
- search apt packages
- explain what layer this belongs in

### Notebook package mismatch hint

For notebooks, detect the classic case:

- package installed in a terminal
- notebook kernel still cannot import it

The guide explains this, but product hints would save a lot of confusion.
