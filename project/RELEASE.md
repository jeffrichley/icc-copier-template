# Release Process

1. Commit all changes and ensure `make checkit` passes.
2. Use `cz bump` to bump version and update CHANGELOG.md.
3. Push tags to trigger PyPI publish via GitHub Actions.
4. Verify release on PyPI and GitHub Pages for docs.
