# Applied Math

Personal study repository: notes, exercises and solutions, organized by topic.

## Structure

| Folder / file | What goes there |
|---|---|
| [notes/](notes/) | One file per concept, grouped by area |
| [exercises/](exercises/) | One file per exercise, same areas as `notes/` |
| [templates/](templates/) | Copy these to start a new note or exercise |
| [resources.md](resources.md) | Books and courses, with the codes used in `source:` |

## Conventions

- **File names**: lowercase, hyphens: `equations.md`, `absolute-value.md`.
- **Exercise files**: `<source>-<section>-ex<NN>.md` using the book's original numbering, e.g. `precalc-9.1-ex06.md`.
  Problems not taken from a book use `custom-<short-name>.md`.
- **Math**: LaTeX, inline `$x^2$` and block `$$ ... $$`.
- **Links**: relative paths between notes and exercises.
- **Exercises have no solutions**: only the problem and space for my own work.

## Searching

Notes and exercises start with a small YAML header, so a text search works as a filter
(`Ctrl+Shift+F` in VS Code):

| To find | Search for |
|---|---|
| Everything on a topic | the topic name, e.g. `substitution` |
| A book section | `ref: "9.1` |
| Hard exercises | `difficulty: hard` |
| Everything from a book | `source: PRECALC` |
