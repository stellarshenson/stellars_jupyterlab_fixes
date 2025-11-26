# Stellars JupyterLab Fixes

[![GitHub Actions](https://github.com/stellarshenson/stellars_jupyterlab_fixes/actions/workflows/build.yml/badge.svg)](https://github.com/stellarshenson/stellars_jupyterlab_fixes/actions/workflows/build.yml)
[![PyPI version](https://img.shields.io/pypi/v/stellars_jupyterlab_fixes.svg)](https://pypi.org/project/stellars_jupyterlab_fixes/)
[![Total PyPI downloads](https://static.pepy.tech/badge/stellars_jupyterlab_fixes)](https://pepy.tech/project/stellars_jupyterlab_fixes)
[![JupyterLab 4](https://img.shields.io/badge/JupyterLab-4-orange.svg)](https://jupyterlab.readthedocs.io/en/stable/)
[![Brought To You By KOLOMOLO](https://img.shields.io/badge/Brought%20To%20You%20By-KOLOMOLO-00ffff?style=flat)](https://kolomolo.com)

Metapackage that installs all Stellars JupyterLab fixes in one command.

## Installation

```bash
pip install stellars_jupyterlab_fixes
```

## Included Fixes

- **jupyterlab_change_ui_font_size_fix** - Fix file browser alignment when changing UI font size
- **jupyterlab_jump_to_definition_fix** - Fix "jump to definition" for notebooks using Jedi in kernel environment
- **jupyterlab_markdown_switch_tab_scrolling_fix** - Prevent markdown scroll drift when switching tabs
- **jupyterlab_markdown_viewer_toc_fix** - Fix broken TOC navigation and anchor links in Markdown Viewer

## Requirements

- JupyterLab >= 4.0.0
- Python >= 3.9
