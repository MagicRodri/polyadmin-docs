# Frontend and rendering

Both implementations render HTML on the server. HTMX replaces list and form
fragments for search, filtering, sorting, pagination, and validation without
requiring a separate SPA or frontend build pipeline.

The built-in templates use Tailwind CSS, Alpine.js, HTMX, and a port of the
shadcn/ui component language. CSS variables provide the color tokens, so an
application can theme the admin or override an individual resource template
without forking the framework.

The rendering extension points differ slightly between Jinja2 and Go
`html/template`; use the language-specific template documentation for those
details.