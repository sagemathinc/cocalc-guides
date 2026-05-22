# Product Notes From Drafting This Guide

These notes are not part of the public guide. They capture product ideas that
became sharper while writing the RootFS management guide.

## Strong Ideas

### RootFS starter checklist

Publishing a RootFS is powerful, but users need a short visible checklist:

- install software and data
- remove temporary files and secrets
- run a tiny verification
- scan the current RootFS
- choose visibility
- publish with version metadata

This could be a guided flow in the Runtime Image panel.

### Course environment template

Instructors should be able to create a course project, publish its RootFS, and
then select that image as the default environment for new student projects.
The guide wants this to feel like a first-class course setup story rather than
a hidden power-user feature.

### Public software environment page

For researchers or library authors, a public RootFS could use a shareable page:
name, description, versions, scan status, tags, example command, and “create
project from this environment.”

### Upgrade trail

Managed RootFS versions already support rollback and supersedes metadata. The
product could make this more visible as a release timeline: current version,
upgrade target, previous version, and projects still pinned to old versions.

## Smaller Ideas

### Clean-before-publish assistant

Codex can inspect shell history, package lists, large files, and obvious
secrets before publishing. A “prepare this RootFS for publishing” action would
fit naturally.

### Storage explanation

Users benefit from a plain-English explanation that managed RootFS images are
shared base environments and do not count against ordinary project disk quota.
This is easy to misunderstand if one thinks only in terms of project files.

### Docker/OCI boundary

The guide needs to explain that advanced OCI image strings exist, but the
managed RootFS catalog is the CoCalc-native path with metadata, sharing,
scanning, rollback, and faster reuse.
