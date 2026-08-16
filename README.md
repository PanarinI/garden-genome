# garden-genome

Four instruction files an AI assistant is handed before it starts working on a project. They load
into every session, the same four in every project, and they cover the four moments where work is
lost:

| file | when it runs | what it does |
|---|---|---|
| `seed` | a project starts | creates one folder with three files: what this project is, where the work stands, why it was decided that way |
| `boker` | a session opens | refreshes the panel, reads the state of one project, names the next step |
| `shabbat` | a session closes | rewrites the state file in meaning, appends the reason to the journal, writes a timestamp |
| `vedro` | any time | appends a stray thought as one line to a bucket file; it is sorted in a later pass, not now |

Between them they hold about two hundred lines. Nothing here is enforced by tooling: the files are
instructions, and the assistant follows them the way it follows any other instruction.

The text is in Russian, the language the work is done in.

Format: [Claude Code skills](https://docs.claude.com/en/docs/claude-code/skills) — one folder per
skill, a `SKILL.md` inside.

How this is used day to day, with the rest of the system around it:
[panarini.github.io/projects/garden.html](https://panarini.github.io/projects/garden.html)
