# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository purpose

A collection of [navi](https://github.com/denisidoro/navi) `.cheat` files — interactive command snippets invoked through `navi`'s fuzzy-finder UI. There is no build system, no test runner, and no source code: each `*.cheat` file at the repo root is a standalone deliverable.

## Working with `.cheat` files

Every file in this repo follows navi's cheatsheet grammar. When adding or editing a cheat, preserve these conventions observed across the existing files:

- **First line is the tag header**: `% <tool>, <category>` (e.g. `% rustscan, network`). The tool name comes first; the second tag is a broad category (`network`, `terminal`, `text`, `process`, `media`, `sync`, `filesystem`, …). Use the same category as similar tools already in the repo.
- **Each snippet is a `#` comment describing *why/what* followed by the command line**. Descriptions are short and imperative ("Scan all ports on a host"), not narration.
- **Placeholders use `<name>` syntax** inside commands and are resolved by `$ name: <provider>` lines at the bottom of the file. Providers fall into two patterns:
  - Dynamic: shell commands that enumerate live values — `fd --type f …`, `tmux ls | cut -d: -f1`, `git log --oneline -n 30`. Always suffix with `2>/dev/null` so the picker doesn't surface stderr.
  - Static: `echo -e "opt1\nopt2\n…"` lists of sensible defaults.
  - Both typically end with `--- --column 1` so navi takes the first whitespace-column as the value.
- **Reuse placeholder names across snippets in the same file** so one `$ name:` provider serves every snippet that references `<name>`. Don't invent `<port_1>` / `<port_2>` when `<port>` will do.
- **Flag accuracy matters**: a recent commit (`40070ed fix(cheats): correct flags and subcommands for lms/tre/procs`) cleaned up incorrect flags. When adding a snippet, verify the flag exists in the tool's current `--help` output rather than trusting memory — several tools in this repo have quirky or renamed flags (`procs --sorta/--sortd`, `lms sync --nodelete`, `tre`'s numbered alias output, etc.).

## Validating a cheat locally

```sh
# Dry-preview: show navi's picker using only this directory's cheats
navi --path . 

# Confirm a specific file parses and lists its snippets
navi --path . --print

# Run navi filtered to one tag (the first token of the % header)
navi --path . --tag-rules <tool>
```

If a `$ placeholder:` provider is broken, navi silently shows an empty list for that variable — always trigger the snippet end-to-end in the picker before committing.

## Keep `README.md` in sync

`README.md` contains a single tools table (`| Tool | Description | Link | Cheatsheet |`) that is the canonical index of this repo. When you add a new `<tool>.cheat`, add a matching row to that table; when you remove one, delete its row. The table order is roughly the order cheats were added, not alphabetical — append new rows at the bottom.

## Commit style

Follow the conventional-commit style already in `git log`:

- `docs(cheats): …` for new or expanded cheats
- `fix(cheats): …` for corrections to flags/subcommands/syntax
- `docs(readme): …` for README-only changes

Scope is almost always `cheats` or `readme`; keep the subject imperative and specific about which tools changed.
