# Pi

Small Pi Coding Agent extensions and skills with narrow responsibilities.

This repo is the index for Pi-related extensions, skills, and conventions. Extension implementations stay in their own repositories. Small skills can live directly in `skills/` until they need their own package or release flow.

## Extensions

| Name | Responsibility | Install |
|---|---|---|
| [Downshift](https://github.com/boadij/pi-downshift) | Starts strong, preserves context, then switches to a cheaper model when context pressure crosses a threshold. | `pi install npm:pi-downshift` |
| [Killswitch](https://github.com/boadij/pi-killswitch) | Requests wrap-up or kills a run when context-budget thresholds are reached. | `pi install pi-killswitch` |

## Skills

Skills live in [`skills/`](./skills/).

A separate repo is only needed when a skill grows into a package, needs its own release flow, or has enough surface area to justify independent issues and docs.

## Design rules

- One narrow responsibility per extension or skill.
- Prefer predictable behavior over broad orchestration.
- Keep extension implementation in its own repo.
- Keep shared conventions here.
- Avoid submodules unless this repo becomes a pinned integration workspace.
- Keep this repo useful without a build step.

## Registry

Machine-readable metadata lives in [`registry.json`](./registry.json).

The registry is intentionally small. It exists so future scripts, docs, installers, or catalog pages can read the same source of truth without scraping this README.

## Templates

Use the templates in [`templates/`](./templates/) when adding a new extension or skill:

- [`templates/extension.md`](./templates/extension.md)
- [`templates/skill.md`](./templates/skill.md)

## Current shape

```text
README.md
registry.json
registry.schema.json
skills/
  README.md
templates/
  extension.md
  skill.md
LICENSE
```
