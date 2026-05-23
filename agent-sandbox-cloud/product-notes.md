# Product Notes

## Positioning choices

- Avoid positioning CoCalc as a Vercel/Railway replacement. Those products are
  public app deployment surfaces; CoCalc is primarily where humans and agents
  work before deployment.
- Avoid saying only "sandbox." Use fuller phrases such as "durable
  collaborative project," "agent-ready project cloud," or "managed Linux
  project workspace."
- Be explicit about the container tradeoff: rootless Podman gives density and
  cost advantages, but it is not the same isolation claim as a microVM product.
- Dedicated managed hosts are a major economic story. The user gets dedicated
  capacity without SSH/root administration of the host.

## Follow-up documentation hooks

- A precise CLI guide for `cocalc project create`, `exec`, `ssh`, `snapshot`,
  `backup`, `move`, and file access while stopped.
- A host economics guide explaining shared pool, dedicated hosts, spot fallback,
  egress guardrails, and self-hosting.
- A security/trust guide comparing rootless containers, project permissions,
  SSH, secrets, egress, snapshots, backups, and public app exposure.

## Product ideas surfaced while writing

- Consider making "develop here, deploy elsewhere" an explicit product surface
  for static sites and web apps.
- Public app exposure should be carefully named and probably separated from the
  main sandbox-cloud narrative so it does not distort positioning.
- The egress monitor deserves visible marketing. Accidental cloud egress is a
  concrete pain that sandbox and agent users understand immediately.
