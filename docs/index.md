# PolyAdmin

PolyAdmin is a server-rendered, Django-admin-style framework for building
internal tools with the language and web stack you already use.

Choose an implementation:

=== "Python / FastAPI"

    Use the Python implementation when your application runs on FastAPI.
    Start with the [Python getting started guide](python/index.md).

=== "Go / Fiber"

    Use the Go implementation when your application runs on Fiber. Start with
    the [Go getting started guide](go/index.md).

Both implementations share the same design:

- Your application owns models, storage, business rules, and authentication.
- PolyAdmin owns the server-rendered admin experience and its routes.
- A `ModelAdmin` declares how one resource is listed, edited, searched, and
  authorized.
- The adapter connects the framework to the host web application.

## What you get

- CRUD with search, filtering, sorting, and pagination
- Dashboard widgets and custom admin pages
- Authentication and per-resource authorization hooks
- Relations, inline records, actions, exports, and delete previews
- HTMX-powered partial updates without a frontend build step
- Internationalization and themeable shadcn/ui-inspired components

The language-specific sections document the public API and adapter contracts;
the shared concepts section explains the architecture behind both libraries.