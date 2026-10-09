# Issue tracker: local Markdown

Product plans, specs, and implementation issues for this repo live as Markdown files under `docs/planning/`.

## Conventions

- Keep one feature per directory: `docs/planning/<feature-slug>/`.
- Put its product plan and spec in that directory.
- Put implementation issues at `docs/planning/<feature-slug>/issues/<NN>-<slug>.md`, numbered from `01` for new feature plans. Use one file per issue.
- Record triage state in a `Status:` line near the top of each issue file. Use the values in `docs/agents/triage-labels.md`.
- Append discussion under a `## Comments` heading.

## When a skill says "publish to the issue tracker"

Create a Markdown issue in the appropriate feature's `issues/` directory. Create the directory if needed.

## When a skill says "fetch the relevant ticket"

Read the issue at the supplied path, or find it by feature and issue number.

## Wayfinding operations

For `/wayfinder`, the map is `docs/planning/<effort>/map.md`, with one child file per ticket at `docs/planning/<effort>/issues/<NN>-<slug>.md`.

- The map holds Notes, Decisions-so-far, and Fog.
- Each child has a `Type:` line (`research`, `prototype`, `grilling`, or `task`) and a `Status:` line (`claimed` or `resolved`).
- Record dependencies near the top as `Blocked by: NN, NN`. A child is unblocked when every listed ticket is resolved.
- To find the next ticket, scan for open, unblocked, unclaimed children. Take the lowest number first.
- To claim a ticket, set `Status: claimed` and save before starting work.
- To resolve it, add the answer under `## Answer`, set `Status: resolved`, and append a brief summary with a link to the ticket under Decisions-so-far in `map.md`.
