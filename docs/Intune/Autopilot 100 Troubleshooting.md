---
tags:
    - Autopilot
    - OOBE
---

# Autopilot level 100 troubleshooting

# My Documentation Website

## Setting up Python environment 🐍
```java
winget install --id=Python.Python.3.14 -e
python --version
where.exe python
```

If python --version shows the version and where.exe python returns the actual path (e.g., C:\Users\<You>\AppData\Local\Programs\Python\Python314\python.exe or C:\Program Files\Python\...), Python is on PATH.

```
python -m venv venv
venv/Scripts/activate
```

## Setting up the Theme (Material)
Activate your virtual environment, then install the Material theme:

```java
# from your project folder, with the venv activated
pip install mkdocs-material
```

`Documentation Link:` https://squidfunk.github.io/mkdocs-material/getting-started/

Add the following lines to `mkdocs.yml` (simple example):

```yaml
theme:
  name: material
  language: en
  features:
    - navigation.instant
    - navigation.top
```

If you previously installed `mkdocs-terminal`, you can uninstall it with:

```powershell
pip uninstall mkdocs-terminal
```

## Additional Themes
- https://github.com/daizutabi/mkdocs-ivory
- https://gitlab.com/lramage/mkdocs-bootstrap386
- https://github.com/ntno/mkdocs-terminal

## Initialization of MKDocs
```
mkdocs new .
```

This created a mkdocs.yml file and a docs folder with index.md

# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Configuring the mkdocs.yml file
```yaml




```
