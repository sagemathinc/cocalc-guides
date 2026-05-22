# Product Notes

## Good follow-up documentation hooks

- A tiny technical drawer for the remote SSH flow:
  `cocalc-plus ssh user@host`, remote install, daemon on `127.0.0.1`, auth token,
  SSH port forward, open local tab.
- A short sync reference for selecting local and remote roots, expected conflict
  behavior, ignore rules, and how to inspect sync logs.
- A trust-model note that explicitly distinguishes Plus from hosted
  project-host sandboxing: Plus runs on machines the user controls and inherits
  that account's authority.
- A provider-facing landing page for Runpod/Nebius/Lambda-style images where
  Plus appears beside JupyterLab as the simple CoCalc option.

## Product ideas surfaced while writing

- The remote launch flow is compelling enough to deserve a first-class visual
  onboarding screen inside Plus, not only CLI help.
- The install page could link directly to this guide so early users understand
  why Plus exists before they run the command.
- The sync UI should expose enough status to make users comfortable: last scan,
  last copy, conflicts, ignored paths, and whether hot watching is active.
