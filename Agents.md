# Silvie image CDN

This repository is a static GitHub Pages CDN. The published root is `docs/`, which contains Grand Archive card images, API snapshots, collection-tracker assets, and shared UI artwork. There is no application build step for the asset tree; the small Node script is only a local `http-server` convenience for previewing `docs/`.

## Working conventions

- Preserve public URL paths when adding or moving assets; consumers reference `https://img.silvie.org/...` directly.
- `docs/cdn/collection-tracker/logo/` contains set logos. The sibling `bot` scraper downloads featured-set logos there from the Grand Archive API.
- `docs/api-data/` contains downloaded card images keyed by edition UUID.
- Check repository status and asset dimensions/file types before replacing an existing image.
