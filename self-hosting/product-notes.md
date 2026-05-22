# Product Notes

These are ideas surfaced while writing the guide.

## The Launchpad page should explain the story, not just the installer

The current public Launchpad install page is intentionally minimal. It should
probably link to this guide or carry a short "why this exists" section:

- tiny single-file install,
- PGlite for one-process control plane,
- first admin account,
- bring your own compute,
- same CoCalc-AI experience as the public cloud,
- Rocket as the scale-up path.

## Self-hosting needs a first-run checklist

After creating the admin account, the product could guide the operator through:

- enable 2FA or passkeys,
- set public signup / registration-token policy,
- configure site title and outbound email,
- connect a project host or provider,
- create a test project,
- set membership tiers and quotas,
- create the first backup policy.

That would make the "one binary" story feel complete.

## Rocket positioning should be explicit early

Launchpad is not a toy if Rocket is the larger deployment sibling. The product
copy should say this directly: Launchpad is for small teams; Rocket is the
enterprise-grade scale-up with the same user-facing functionality and a larger
control-plane/deployment footprint.

## Security page for operators

Self-hosted operators need a compact security dashboard that says:

- 2FA/passkey status,
- fresh-auth policy,
- registration policy,
- project-secret usage,
- public app exposure,
- cloud provider credentials configured,
- backup health,
- dangerous-action audit log.

This is partly present in pieces; the self-hosting story makes the need more
obvious.
