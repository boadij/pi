# Extension template

Use this shape when adding a Pi extension to the catalog.

## Registry entry

```json
{
  "name": "pi-example",
  "displayName": "Example",
  "type": "extension",
  "repo": "https://github.com/boadij/pi-example",
  "install": "pi install pi-example",
  "category": "example-category",
  "summary": "One sentence describing the narrow responsibility.",
  "status": "experimental"
}
```

## README entry

```md
| [Example](https://github.com/boadij/pi-example) | One sentence describing the narrow responsibility. | `pi install pi-example` |
```

## Checklist

- The extension has one narrow responsibility.
- The extension has its own repo.
- The install command is documented.
- The README explains what it does and what it does not do.
- The registry entry validates against `registry.schema.json`.
