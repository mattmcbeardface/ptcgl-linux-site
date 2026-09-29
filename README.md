# PTCGL-Linux website

Website and signed Flatpak repository for PTCGL-Linux.

Production site: https://ptcgl-linux.com

The www.ptcgl-linux.com hostname permanently redirects to the apex domain.

## Website

The site is a static Cloudflare Pages deployment connected to this repository.

Primary files:

- index.html — one-page website
- styles.css — responsive styling
- assets/hero.webp — optimized hero background
- _headers — Cloudflare Pages response headers

There is no application build step.

## Flatpak distribution

Signed Flatpak repository:

    https://ptcgl-linux.com/flatpak/repo/

Public installer:

    https://ptcgl-linux.com/flatpak/Pokemon-TCG-Live.flatpakref

Stable application ref:

    app/io.github.PTCGLLinux/x86_64/stable

The Flatpak repository is GPG signed.

Never commit the private repository signing key.

## Deployment

Cloudflare Pages deploys automatically from the main branch.

The repository root is the Pages output directory.

## Local preview

Run:

    python3 -m http.server 8080

Then open:

    http://localhost:8080
