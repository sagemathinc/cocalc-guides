# Product Notes

## Positioning choices

- Overleaf should remain the main familiar reference point. Many potential
  CoCalc users already love it, so the comparison should start from respect:
  hosted collaboration, low setup, and visual editing are real strengths.
- CoCalc's strongest LaTeX claim is not "a better LaTeX editor." It is "the
  paper lives in the same durable project as the computation, terminal,
  TimeTravel, chat, collaborators, and Codex."
- CoCalc Plus is worth highlighting because it gives a local/private LaTeX
  editing shape with TimeTravel and Codex integration, which is uncommon among
  hosted LaTeX tools.

## Follow-up documentation hooks

- A technical drawer for build-aware Codex help: last LaTeX build log, source
  file, bibliography warnings, missing references, and exact rebuild command.
- A short recipe for computational papers: Jupyter or scripts generate figures
  and tables, LaTeX consumes them, Codex checks stale references and captions.
- A "paper review with Git Review" guide focused on mathematical/technical
  authors who want careful line-level review of agent-generated edits.

## Product ideas surfaced while writing

- The LaTeX editor should expose the last build log to Codex through a clean
  `cocalc project latex` CLI, not only through browser memory.
- A first-run LaTeX workspace template could include `paper.tex`,
  `figures/`, `notebooks/`, `scripts/`, `references.bib`, and a Codex prompt
  for explaining the project structure.
- CoCalc Plus could be marketed directly to local LaTeX authors who want
  TimeTravel and AI help without uploading papers to a hosted writing service.
