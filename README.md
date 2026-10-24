# Bullish Ideas

Bullish Ideas collects early concepts, experiments, and writing about design and technology.

## Site structure

- `content/_index.md` sets the homepage sections.
- `content/portfolio/` holds ideas and the public `/ideas/` list.
- `content/about/` and `content/contact/` hold the site pages.
- `static/images/` holds the logo variants, favicon, and editorial artwork.
- `.siteman/` holds Hugo settings, theme defaults, and site layout overrides.

## Theme and visual settings

The site uses Roxo Flex first, with Siteman Default as a fallback. Theme settings live in `.siteman/hugo.toml`. The palette uses paper `#F6F2E8`, charcoal `#242724`, muted text `#555B54`, and gold sampled from the logo grid.

The sampled gold is `#E5B866`. The logo uses it on charcoal. The site uses its darker shade `#93620F` for links and buttons on paper. Contrast is 13.51:1 for charcoal on paper, 6.24:1 for muted text on paper, 4.70:1 for gold text on paper, 5.26:1 for white on gold buttons, and 8.18:1 for logo gold on charcoal.

The header uses the horizontal logo. The footer uses the stacked logo. The favicon uses the circular icon. `static/images/mark.svg` is the editable vector mark.

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
