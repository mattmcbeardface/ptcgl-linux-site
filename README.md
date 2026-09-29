# PTCGL-Linux website

Static one-page website for PTCGL-Linux.

## Files

- `index.html` — complete one-page site
- `styles.css` — responsive styling
- `assets/hero.webp` — optimized hero background
- `assets/hero.png` — original PNG fallback/source

## Deploy

This site has no build step and no runtime dependencies.

For Cloudflare Pages, connect the GitHub repository as a Pages project and publish the repository root as static files. No framework or build command is required.

## Download link

The current download button points to:

`https://github.com/mattmcbeardface/ptcgl-linux/releases`

When the Flatpak repository / `.flatpakref` is published, replace that URL in `index.html` with the direct installation link.

## Local preview

From this directory:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.
