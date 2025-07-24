# QUICKSTART for ICC Copier Template

This repository contains the **`icc-copier-template`** used to bootstrap new AI, agent, and video-gen projects with Jeff's standards.

---

## 1. Generate a New Project
```bash
uvx copier copy gh:YourGitHubUser/icc-copier-template my-new-project
cd my-new-project
uv sync --extra dev
pre-commit install
make checkit
