# UFN Autoconnect Generator

A static GitHub Pages utility for building EmptyEpsilon autoconnect links.

## Current features

- Automatically detects the viewer's public/external IPv4 address when the page opens
- External address remains fully editable
- Refresh IP control to re-detect the current public IPv4 address
- Server password defaults to `sxp` but remains editable
- Batch player-name entry, one per line or comma-separated
- Player name is passed as the `callsign` query parameter
- Duplicate player names are ignored
- Compact generated-link rows
- Individual Copy Link button for every player
- Correct URL encoding
- UFN navy/gold Systems styling using the supplied UFN logo

## Public IP lookup

The page attempts to retrieve the viewer's public IPv4 address from `api4.ipify.org`, with `api.ipify.org` as a fallback. Only the public-IP lookup request is sent to that service. The server password, player names and generated URLs remain in the browser.

If the lookup fails, the External Server Address field stays editable for manual entry.

## GitHub Pages

1. Upload `index.html` and `ufn-logo.png` to the root of the GitHub repository.
2. Open **Settings → Pages**.
3. Choose **Deploy from a branch**.
4. Select the main branch and `/ (root)`.
5. Save.

## Security note

The EmptyEpsilon autoconnect format places the server password directly in the generated URL. Anyone who receives the URL can read that password from the query string.
