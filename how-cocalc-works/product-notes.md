# Product Notes

This guide explains the architecture without becoming an operator manual.

## Claims To Keep Accurate

- A bay is a control-plane cell: Node.js services plus its own Postgres database.
- Launchpad is the one-bay version of the same architecture.
- Rocket runs the same code with Postgres, many systemd services, and multiple
  bays.
- Project hosts are the compute/data-plane machines where project containers
  run.
- Browser project traffic connects directly to project hosts with short-lived
  host-scoped credentials.
- Project/document sync services can operate even when a project runtime is off.
- Sync state is stored as ordinary SQLite files in the project.
- Cloudflare R2 plus Rustic is used for project backups, Postgres backups,
  RootFS storage, and moving/copying project state across hosts and regions.
- CoCalc currently uses systemd for bays/Rocket and rootless Podman on project
  hosts, not Kubernetes.

## Useful Source Anchors

- `src/.agents/scalable-architecture.md`
- `src/.agents/bay-systemd-deployment-plan.md`
- `src/.agents/project-host-conat-service-split-plan.md`
- `docs/project-host-auth.md`
- `docs/sync.md`
- `docs/ssh-proxy.md`
- `src/packages/project-host`
- `src/packages/file-server`
- `src/packages/conat`
