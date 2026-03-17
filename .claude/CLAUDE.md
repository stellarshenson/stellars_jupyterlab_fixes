<!-- @import /home/lab/workspace/.claude/CLAUDE.md -->

# Project-Specific Configuration

This file imports workspace-level configuration from `/home/lab/workspace/.claude/CLAUDE.md`.
All workspace rules apply. Project-specific rules below strengthen or extend them.

The workspace `/home/lab/workspace/.claude/` directory contains additional instruction files
(MERMAID.md, NOTEBOOK.md, DATASCIENCE.md, GIT.md, and others) referenced by CLAUDE.md.
Consult workspace CLAUDE.md and the .claude directory to discover all applicable standards.

## Mandatory Bans (Reinforced)

The following workspace rules are STRICTLY ENFORCED for this project:

- **No automatic git tags** - only create tags when user explicitly requests
- **No automatic version changes** - only modify version in package.json/pyproject.toml/etc. when user explicitly requests
- **No automatic publishing** - never run `make publish`, `npm publish`, `twine upload`, or similar without explicit user request
- **No manual package installs if Makefile exists** - use `make install` or equivalent Makefile targets, not direct `pip install`/`uv install`/`npm install`
- **No automatic git commits or pushes** - only when user explicitly requests

## Project Context

**stellars_jupyterlab_fixes** - Python metapackage aggregating all Stellars JupyterLab fixes.

**Technology Stack**:
- Python >= 3.10
- JupyterLab >= 4.0.0
- Hatchling build system
- PyPI distribution

**Package Dependencies** (all Stellars fixes):
- jupyterlab_change_ui_font_size_fix
- jupyterlab_jump_to_definition_fix
- jupyterlab_markdown_switch_tab_scrolling_fix
- jupyterlab_markdown_viewer_toc_fix
- jupyterlab_other_file_type_menu_fix
- jupyterlab_server_proxy_launcher_fix
- jupyterlab_terminal_cpr_escape_fix

**Build Commands**:
- `make build` - Build the package (increments version)
- `make install` - Install locally (increments version)
- `make publish` - Publish to PyPI (increments version)
- `make clean` - Remove build artifacts
- `make uninstall` - Uninstall the package
