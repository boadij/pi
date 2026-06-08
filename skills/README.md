# Skills

Small Pi skills can live here when they do not need a separate package or repository.

Use a separate repo only when a skill needs its own release flow, has substantial docs, or becomes useful outside this collection.

## Layout

Each skill should use its own folder:

```text
skills/
  my-skill/
    README.md
```

## Rules

- Keep one narrow responsibility per skill.
- Keep the README short and operational.
- Prefer plain text and Markdown unless the skill needs code.
- Move the skill to its own repo if it starts behaving like a package.

## Registry

When a skill is added, also add it to [`../registry.json`](../registry.json) with `type: "skill"` and a local `path`.
