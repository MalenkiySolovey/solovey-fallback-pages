# Solovey Fallback Pages

Static decoy page templates for the Solovey UI `fallback-html` component.

The panel downloads this repository catalog at:

```text
https://raw.githubusercontent.com/MalenkiySolovey/solovey-fallback-pages/main/templates/catalog.json
```

## Structure

```text
templates/
  catalog.json
  <template-id>/
    manifest.json
    pages/
      index.html
      404.html
    assets/
      site.css
```

Each template is a static HTML/CSS package. The panel copies pages and assets into the local component storage before publishing a site.

## Safety Rules

- No JavaScript.
- No forms, inputs, iframes, embeds, objects, or base tags.
- No inline event handlers.
- No remote CSS imports or remote asset URLs.
- Local navigation links are allowed.
- External HTTPS links are allowed only as ordinary `<a href="...">` links.
- Templates should look like normal low-risk public pages and must not expose panel routes, API paths, subscription paths, or Solovey UI branding.

## Sources

The current templates are hand-adapted static pages inspired by MIT-licensed dashboard/template projects stored locally under `upstreams/FallbackHTML`. Runtime framework code from those projects is not copied here.

## Templates

- `webmail-workspace`: mailbox-like workspace surface.
- `file-vault`: file workspace surface.
- `status-dashboard`: status dashboard surface.
