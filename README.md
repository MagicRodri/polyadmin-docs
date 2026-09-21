# PolyAdmin documentation

Shared documentation for the Python/FastAPI and Go/Fiber PolyAdmin libraries.

The site is built with MkDocs Material and deployed to GitHub Pages by the
workflow in `.github/workflows/docs.yml`.

The adapter reference pages are copied from the implementation repositories at
build time so this site can document both projects without making either one
the owner of the documentation site.

## Cross-repository updates

The Python and Go repositories notify this site when files under their `docs/`
directories change. Add a repository secret named `DOCS_REPO_TOKEN` to both
repositories. The token must be able to dispatch workflows in
`MagicRodri/polyadmin-docs`.

The site also rebuilds nightly, which picks up source documentation changes if
a notification is ever missed.

## Local preview

```bash
uvx --from mkdocs-material mkdocs serve
```