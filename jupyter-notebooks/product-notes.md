# Product Notes

These are ideas surfaced while writing the guide.

## Build a notebook assistant status rail

The `cocalc project jupyter` interface gives Codex a strong way to work with
live notebook state. The notebook UI could expose a small status rail showing
the latest agent interactions with the notebook:

- cells Codex inspected,
- cells Codex inserted or modified,
- run IDs Codex started,
- output/error summaries Codex used,
- links back to the chat turn that caused each action.

This would make agent edits feel auditable without forcing users to inspect raw
chat logs.

## Make TimeTravel output policy visible

The guide explains that TimeTravel should keep final output state without
storing every transient streaming step. It would help to make this explicit in
the UI when looking at notebook history: "final output preserved" versus "live
stream omitted".

## Whiteboard graph execution deserves a mini guide

Jupyter cells in a directed whiteboard graph are unusual and strong enough to
deserve their own small guide or product tour. The story is different from a
linear notebook: pipelines, dependency structure, teaching diagrams, and
interactive computational maps.

## Notebook provenance could connect all the pieces

The strongest product direction is a unified provenance trail:

- TimeTravel edits,
- cell execution runs,
- Codex notebook actions,
- collaborator attribution,
- whiteboard graph runs,
- nbgrader/course events.

This does not need to be noisy in the notebook itself, but it would give users a
clear answer to "who changed what, what ran, and why does this output exist?"
