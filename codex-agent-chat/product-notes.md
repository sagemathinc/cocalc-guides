# Product Notes: Codex Agent Chat

Writing this guide suggests a few product hooks that would make the story easier
to teach without making the guide heavier.

## Capability receipt

Each Codex thread could expose a compact "what this agent can use" receipt:

- payment source: ChatGPT plan, account key, project key, site key, or shared
  setup
- session mode: read-only, workspace-write, or full-access
- project tools: terminal, Jupyter, text sync, browser state, image generation
- working directory and project id

This would make collaboration and audits easier because users could see the
execution context without reading implementation details.

## Thread templates

The guide wants a few named templates:

- paper review
- bug investigation
- long computation monitor
- release checklist
- scheduled notebook check

Templates would mostly be prefilled thread settings plus a first prompt.

## Automation dashboard

Scheduled Codex runs are strong, but discoverability could improve if a project
had one view listing all chat automations, next run times, paused state, and last
unacknowledged result.

## Secrets bridge

The story around Project Secrets is good. It would be useful for guides to link
to a stable recipe page or in-product anchor for "generate encrypted project SSH
key" and "store project API key."
