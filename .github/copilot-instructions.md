# GitHub Copilot Instructions

This file provides GitHub Copilot with context about the **Mu-files** repository so it can give accurate, relevant suggestions when working on any file here.

## Repository Purpose

`Mu-files` is a personal file repository used to store, organize, and version-control various files. GitHub Copilot is enabled here to assist with:
- Improving and enhancing existing files
- Writing new scripts, config files, and documentation
- Refactoring or restructuring file content

## Repository Layout

| Path | Description |
|------|-------------|
| `config/` | Configuration files (JSON, YAML, TOML, environment templates) |
| `docs/` | Documentation, notes, guides, and reference materials |
| `scripts/` | Shell scripts, Python utilities, and automation helpers |
| `.github/` | GitHub-specific files including these Copilot instructions |

## Conventions

### General
- Prefer clear, self-documenting names for files and variables.
- Add a brief comment at the top of each file explaining its purpose.
- Keep files focused on a single concern.

### Scripts
- Shell scripts should start with `#!/usr/bin/env bash` and include `set -euo pipefail`.
- Python scripts should include a `if __name__ == "__main__":` guard.
- Add a usage/help comment block near the top of every script.

### Configuration Files
- JSON files should be pretty-printed (2-space indentation).
- YAML files should use 2-space indentation and include comments for non-obvious keys.
- Avoid committing secrets or credentials; use `.env.example` templates instead.

### Documentation
- Markdown files should use ATX-style headings (`#`, `##`, `###`).
- Include a short summary paragraph at the top of each doc file.
- Use tables for structured data and fenced code blocks for code examples.

## How to Use Copilot in This Repo

1. **Inline suggestions** – Open any file and start typing; Copilot will suggest completions that match the conventions above.
2. **Copilot Chat** – Ask questions like "Improve this script" or "Add error handling to this function" and Copilot will use this file as context.
3. **Edits** – Use Copilot Edits to apply larger refactors across multiple files while staying consistent with the repo conventions.
