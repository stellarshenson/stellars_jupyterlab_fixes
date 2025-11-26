<!-- Import workspace-level CLAUDE.md configuration -->
<!-- See /home/lab/workspace/.claude/CLAUDE.md for complete rules -->

# Project-Specific Configuration

This file extends workspace-level configuration with project-specific rules.

## Project Context

**stellars_jupyterlab_fixes** - Python metapackage aggregating all Stellars JupyterLab fixes.

**Technology Stack**:
- Python >= 3.9
- JupyterLab >= 4.0.0
- Hatchling build system
- PyPI distribution

**Package Dependencies** (all Stellars fixes):
- jupyterlab_change_ui_font_size_fix
- jupyterlab_jump_to_definition_fix
- jupyterlab_markdown_switch_tab_scrolling_fix
- jupyterlab_markdown_viewer_toc_fix

**Build Commands**:
- `make build` - Build the package
- `make install` - Install locally
- `make publish` - Publish to PyPI
