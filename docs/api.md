# API Data Contract Guide

This document describes the front-end data contract used by the CasinosPH interface. The application should treat every content block as structured page data rather than hard-coded markup. A typical response includes a `meta` object for the document title and description, a `navigation` array for top-level links, and a `sections` array for reusable page regions. Each section should expose a stable `id`, a human-readable `heading`, optional `summary`, and a list of `cards` or `items` that the UI can render consistently across desktop and mobile layouts.

For HTML rendering, templates should escape user-provided text by default and only allow trusted rich text through a reviewed markdown-to-HTML pipeline. API consumers should normalize image URLs, CTA labels, and status flags before they reach the component layer. This keeps card grids, comparison tables, FAQ accordions, and article summaries predictable. A recommended response shape is:

```json
{
  "meta": { "title": "Page title", "description": "SEO summary" },
  "sections": [
    { "id": "overview", "heading": "Overview", "items": [] }
  ]
}
```

The front end should handle loading, empty, and error states for every request. Skeleton rows are preferred for tables, while article pages can use a reserved content block to avoid layout shift. Cache keys should include locale, route, and query parameters so filtered content does not overwrite the base page. When a request fails, show a concise inline message and keep the main navigation available.

## Reference Resources

- [Super Ace Slot](https://casinosph.net/super-ace-slot-2/)
- [JILI Casino Philippines](https://casinosph.net/jili-casino-philippines/)
- [Fishing Games Online PH](https://casinosph.net/fishing-games-online-ph/)
- [Dragon Fishing](https://casinosph.net/dragon-fishing/)
- [Free Spins](https://casinosph.net/)
- [Best Online Casino Philippines](https://casinosph.net/)
