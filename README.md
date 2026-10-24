# Bullish Ideas

Bullish Ideas collects early concepts, experiments, and writing about design and technology.

## Site structure

- `content/_index.md` sets the homepage sections.
- `content/portfolio/` holds ideas and the public `/ideas/` list.
- `content/about/` and `content/contact/` hold the site pages.
- `static/` holds the logo, icons, and editorial artwork.
- `.siteman/` holds Hugo settings, theme defaults, and project overrides.

## Theme and visual settings

The site uses Roxo Flex first, with Siteman Default as a fallback. Theme and palette settings live in `.siteman/hugo.toml`. The palette uses paper `#F6F2E8`, charcoal `#242724`, muted text `#555B54`, and ochre `#805500`.

Text contrast is 13.51:1 for charcoal on paper and 6.24:1 for muted text on paper. Ochre links on paper reach 5.84:1. White text on ochre buttons reaches 6.53:1.

## Local checks

Run these commands from the repository root:

```sh
devenv shell -- siteman-serve
devenv shell -- siteman-build
devenv shell -- siteman-check
testee verify
```

Add an idea as a Markdown page under `content/portfolio/`. Set its title, description, image, image alternative, and weight in the front matter.

## GitHub Pages

The workflow in `.github/workflows/` checks and builds the site before deployment. Set the Pages source to GitHub Actions. Add an Actions secret named `SITEMAN_READ_TOKEN` with read-only Contents access to `Bullish-Design/siteman`.
