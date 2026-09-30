# Repository guidance

This repository currently contains AI contribution guidance and documentation; `README.md` is its onboarding documentation, with no separate docs site. It has no application code or configured build, lint, or test commands. Do not invent project-specific commands or conventions.

## Done means

- `git diff --check` passes.

## Never merges without a human

A person has to have **read this diff** before it lands. Telling an agent "merge it when you're done" is approving a goal, not this change — so it does not count for anything on this list. Everywhere else it counts fine, which is the point of having a list.

No repository-specific high-risk paths are currently present.

## Documentation

Keep the purpose, contributor guidance, and installed skill source in `README.md` accurate. The canonical contribution guidance is this file; tool-specific instruction files should point here rather than duplicate it.

## Maintenance matrix

| Change | Also update |
|---|---|
| `AGENTS.md` | `.github/copilot-instructions.md` must continue to point here. |
| `.agents/skills/ai-ready/` | `skills-lock.json` must match the installed skill; `README.md` must link to the installed skill and its source. |
