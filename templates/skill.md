# Skill template

Use this shape when adding a small skill to `skills/`.

## Folder layout

```text
skills/example-skill/
  README.md
```

## Skill README

```md
# Example Skill

One sentence describing the narrow responsibility.

## Use when

- The agent needs to do one specific kind of task.

## Do not use when

- The task needs a full extension or package.

## Instructions

Describe the skill's behavior here.
```

## Registry entry

```json
{
  "name": "example-skill",
  "displayName": "Example Skill",
  "type": "skill",
  "path": "skills/example-skill",
  "category": "example-category",
  "summary": "One sentence describing the narrow responsibility.",
  "status": "experimental"
}
```

## Checklist

- The skill has one narrow responsibility.
- The skill can live as Markdown or lightweight local files.
- The skill has a short README.
- The skill is listed in `registry.json`.
- The registry entry validates against `registry.schema.json`.
