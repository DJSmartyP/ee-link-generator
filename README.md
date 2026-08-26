# UFN Autoconnect Generator

A static browser-based utility for creating EmptyEpsilon autoconnect links in this format:

`https://ee.ufn.systems/autoconnect.html?serveraddress=...&server_password=...&callsign=...`

## Features

- Server IP/address field
- Server password field
- Batch callsign entry (one per line or comma-separated)
- Duplicate callsigns automatically removed
- Correct URL encoding
- Individual copy button for every generated link
- Mobile-friendly UFN Systems styling
- No server-side code
- No dependencies
- Values are processed locally in the browser

## GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html` from this package to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select your main branch and `/ (root)`.
6. Save.

GitHub will provide the public Pages URL.

## Notes

The generated URL includes the server password in the query string because that is how the UFN autoconnect endpoint is structured. Anyone who has the generated link can therefore read that password from the link.


## Default values

- Server address: `192.168.1.240`
- Server password: `sxp`

Both defaults remain fully editable in the form.
