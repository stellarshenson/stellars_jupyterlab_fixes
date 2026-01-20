# Stellars JupyterLab Fixes

[![GitHub Actions](https://github.com/stellarshenson/stellars_jupyterlab_fixes/actions/workflows/build.yml/badge.svg)](https://github.com/stellarshenson/stellars_jupyterlab_fixes/actions/workflows/build.yml)
[![PyPI version](https://img.shields.io/pypi/v/stellars_jupyterlab_fixes.svg)](https://pypi.org/project/stellars_jupyterlab_fixes/)
[![Total PyPI downloads](https://static.pepy.tech/badge/stellars_jupyterlab_fixes)](https://pepy.tech/project/stellars_jupyterlab_fixes)
[![JupyterLab 4](https://img.shields.io/badge/JupyterLab-4-orange.svg)](https://jupyterlab.readthedocs.io/en/stable/)
[![Brought To You By KOLOMOLO](https://img.shields.io/badge/Brought%20To%20You%20By-KOLOMOLO-00ffff?style=flat)](https://kolomolo.com)

Metapackage that installs all Stellars JupyterLab fixes in one command.

These fixes address papercuts and annoyances in JupyterLab 4 that were bothering us enough to do something about them. They are intended as temporary workarounds until the JupyterLab team incorporates proper solutions into the mainline - at which point this repo will happily become obsolete.

> [!WARNING]
> These fixes monkey-patch JupyterLab internals and may break with future JupyterLab updates. Use at your own risk. If something explodes, you get to keep both pieces.

*Yes, we wrote an entire metapackage just to fix scroll positions and font alignments. No, we don't have better things to do. Okay, we do, but here we are.*

## Installation

```bash
pip install stellars_jupyterlab_fixes
```

## Included Fixes

- [jupyterlab_change_ui_font_size_fix](https://github.com/stellarshenson/jupyterlab_change_ui_font_size_fix) - Fix file browser alignment when changing UI font size
- [jupyterlab_jump_to_definition_fix](https://github.com/stellarshenson/jupyterlab_jump_to_definition_fix) - Fix "jump to definition" for notebooks using Jedi in kernel environment
- [jupyterlab_markdown_switch_tab_scrolling_fix](https://github.com/stellarshenson/jupyterlab_markdown_switch_tab_scrolling_fix) - Prevent markdown scroll drift when switching tabs
- [jupyterlab_markdown_viewer_toc_fix](https://github.com/stellarshenson/jupyterlab_markdown_viewer_toc_fix) - Fix broken TOC navigation and anchor links in Markdown Viewer
- [jupyterlab_server_proxy_launcher_fix](https://github.com/stellarshenson/jupyterlab_server_proxy_launcher_fix) - Fix SVG icon display for jupyter-server-proxy launchers in custom categories

## Requirements

- JupyterLab >= 4.0.0
- Python >= 3.9
