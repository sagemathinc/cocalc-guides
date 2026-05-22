# Product Notes: Git Review Workflow

Writing this guide suggests a few product hooks that would make the workflow
clearer and more powerful.

## Review coverage map

A compact project-level view could show reviewed/unreviewed commits across the
current branch, with counts for draft, submitted, and resolved inline comments.
This would make it harder to miss one commit in a long agent session.

## Follow-up commit linking

When inline comments are sent to Codex and the agent makes a fix commit, the
review record could link the original comment submission to the follow-up
commit. That would make "review the fix before marking the original done" a
first-class workflow.

## Batch review prompts

The current one-commit target is clean and precise. For some workflows, it would
be useful to collect draft comments across several commits and ask Codex to
address them in one structured turn while preserving the per-commit targets.

## Stale comment detection

Inline comments already keep hunk and snippet context. The UI could warn when a
comment is being viewed against a changed or rebased commit where the hunk no
longer matches the original review anchor.
