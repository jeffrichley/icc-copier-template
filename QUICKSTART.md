# QUICKSTART for ICC Copier Template

This repository contains the **`icc-copier-template`** used to bootstrap new AI, agent, and video-gen projects with Jeff's standards.

---

## 1. Generate a New Project

```bash
# Create a new project from the template
uvx copier copy gh:jeffrichley/icc-copier-template my-new-project

# Navigate to the new project directory
cd my-new-project

# Install dependencies
uv sync --extra dev

# Install pre-commit hooks
pre-commit install

# Run initial checks to ensure everything is working
make checkit
```

During the copier setup, you'll be prompted for:
- **Project Name**: Human-readable name (e.g., "My Awesome Project")
- **Project Slug**: URL-friendly name (e.g., "my-awesome-project")
- **Package Slug**: Python import name (e.g., "my_awesome_project")
- **Description**: Brief project description

---

## 2. Project Structure

The template creates a standardized project structure:

```
my-new-project/
├── src/
│   └── your_package_name/
│       └── __init__.py
├── tests/
├── docs/
├── scripts/
├── pyproject.toml
├── Makefile
└── README.md
```

---

## 3. Available Commands

The template includes a comprehensive Makefile with common development tasks:

```bash
# Run all checks (format, lint, test, type check)
make checkit

# Format code with black and ruff
make pristine

# Run tests
make test

# Check test coverage
make coverage-check

# Type checking with mypy
make mypy

# Install pre-commit hooks
make install-hooks
```

---

## 4. Agent OS (Optional)

Once the project has been initialized with the template, you can optionally install the Agent OS helper system:

```bash
curl -sSL https://raw.githubusercontent.com/buildermethods/agent-os/main/setup-cursor.sh | bash
```

This provides additional development tools and integrations for AI/agent projects.

---

## 5. Next Steps

1. **Review the generated code** in `src/your_package_name/`
2. **Update the README.md** with your project-specific information
3. **Add your first feature** following the established patterns
4. **Run `make checkit`** before committing to ensure code quality
5. **Check `TODOS.md`** for any project-specific tasks

---

## Troubleshooting

- **Template variables not rendered**: Ensure you completed the copier setup prompts
- **Pre-commit hooks failing**: Run `make pristine` to format code first
- **Coverage issues**: Add tests to reach the 80% coverage requirement

For more details, see the main project documentation in the generated project's `docs/` directory.