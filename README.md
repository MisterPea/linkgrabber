# <img src="images/link_go_32.png" alt="Linkfink icon" width="25" height="25" /> Linkfink  #


Linkfink is a Chrome extension that extracts every hyperlink
from the current page and lists them in a new tab, so you can scan, filter,
and open them in bulk.

### Features ###

- One-click link extraction from the active tab via the toolbar button
- Preset filter options for:
  - Text-fragment links (`#:~:text=`)
  - Same-origin
  - Same-origin sub-domain
  - Duplicate links
- Supports user-specified url block list
- When opening links, user can choose whether links open in new tabs or new windows
- Light / Dark / Auto color mode
- Works in Incognito windows (split mode)

### Development ###

Requires Node.js. Install dependencies with `npm install`.

- `npm run build` — typecheck and build (`js/`, compiled styles)
- `npm run watch` — rebuild on file changes
- `make package` — build and zip the extension into `dist/linkfink.zip`
- `make lint` — run ESLint over `src`

Source lives in `src/` (TypeScript/React + SCSS), compiling to `js/` and
`style/`. To load the unpacked extension in Chrome: run a build, then go to
`chrome://extensions`, enable Developer Mode, and "Load unpacked" pointing
at this repository's root.

See [CHANGELOG.md](CHANGELOG.md) for release history.

### Fork ###

This is a fork of the original Link Grabber by Don Tong
(https://chrome.google.com/webstore/detail/link-grabber/caodelkhipncidmoebgbbeemedohcdma,
https://github.com/7fffffff/linkgrabber). The original author was contacted
about contributing changes upstream but declined, so this fork continues
development independently under a new name, under the terms of the MIT
License.

### Licenses ###

This project is open source software that also bundles other open source
software.

Unless otherwise noted, the MIT License applies.
