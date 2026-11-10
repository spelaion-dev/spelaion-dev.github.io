# spelaion.dev

The website of [Spelaion](https://spelaion.dev): one page about
[SpelaionDB](https://github.com/spelaion-dev/spelaiondb), with download links for its latest
release, and the JSON schemas of SpelaionDB's configuration files.

- Plain HTML and CSS, no build step, served by GitHub Pages at `spelaion.dev` (`CNAME`). To see
  it on your computer: `python3 -m http.server` in this folder.
- The download links ask GitHub's API for the latest release: the main button offers the
  installer for the visitor's system and the Install section links every installer. Without
  JavaScript they open the latest release's page.
- `schema/db/*.schema.json` are copies of SpelaionDB's `schema/` folder, published at
  `https://spelaion.dev/schema/db/`, the URL its configuration files name. Copy them again, from
  the released version, when they change there.

## Brand

The logos and colors come from [`spelaion-dev/brand`](https://github.com/spelaion-dev/brand).
Change a logo there first, then copy it here.

- `logos/*.svg` are copies of that repository's `logos/` files, and `icon.svg` is a copy of
  `logos/spelaion-light.svg`. The page shows the light tile on its light theme and the dark tile
  on its dark one.
- `favicon.png` (64px) and `icon-256.png` are `icon.svg` rendered with
  `rsvg-convert -w 64 -h 64 icon.svg -o favicon.png`. `apple-touch-icon.png` (180px) is the same
  mark on a limestone square with no margin, because iOS cuts the corners itself.
- `og.png` is the card shown when the site is shared: `rsvg-convert og.svg -o og.png`.
- The colors are the first lines of the `<style>` of `index.html` and `404.html`.
- `screenshots/` are copies of SpelaionDB's `docs/screenshots/sdb-46/after-plan-tree-*-1400.png`.

License: Apache-2.0, like SpelaionDB.
