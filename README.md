# spelaion.dev

The website of [Spelaion](https://spelaion.dev): for now a "coming soon" page with a download
button for the latest [SpelaionDB](https://github.com/spelaion-dev/spelaiondb) release, and the
JSON schemas of SpelaionDB's configuration files.

- Plain HTML and CSS, no build step, served by GitHub Pages at `spelaion.dev` (`CNAME`).
- The download button asks GitHub's API for the latest release and offers the installer for the
  visitor's system; without JavaScript it opens the latest release's page.
- `schema/db/*.schema.json` are copies of SpelaionDB's `schema/` folder, published at
  `https://spelaion.dev/schema/db/`, the URL its configuration files name. Copy them again when
  they change there.

License: Apache-2.0, like SpelaionDB.
