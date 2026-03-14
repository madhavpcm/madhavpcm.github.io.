# Portfolio Hugo Site

## Overview

This is a Hugo-based static site using the PaperMod theme. It's a personal portfolio/blog website.

## Project Structure

```
/home/madhavpcm/Dev/kawaserver/servers/portfolio/
├── content/              # Hugo content (markdown files)
│   ├── blog/            # Blog posts
│   │   ├── _index.md    # Blog section config
│   │   └── nginx-rtmp/ # Individual blog post (page bundle)
│   ├── about/           # About page
│   └── cv/              # CV page
├── layouts/             # Custom layouts (overrides theme)
│   └── partials/        # Partial templates
├── static/               # Static assets (images, favicons)
├── themes/PaperMod/     # Hugo PaperMod theme
├── hugo.yaml            # Hugo configuration
├── flake.nix            # Nix flake for dev environment
└── shell.nix            # Legacy nix shell config
```

## Development

To enter the dev environment:
```bash
nix develop -c zsh
```

Then run the Hugo server:
```bash
hugo server -D
```

The site runs at http://localhost:1313

## Build

```bash
hugo -D
```

Output goes to `public/` directory.
