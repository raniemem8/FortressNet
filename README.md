# FortressNet

Graduation project website: Automated Network Threat Detection & Dynamic Malware Analysis
(GNS3, Security Onion, Suricata, Zeek, isolated Python/AI malware sandbox).

Static site: no build step. `index.html` is at the repository root, all paths are relative.

## Deploy on GitHub Pages
1. Create a new GitHub repository (for example `FortressNet`).
2. Upload everything in this folder to the repository root (keep `index.html` at the top level).
3. Go to **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
5. After a minute the site is live at `https://<your-username>.github.io/FortressNet/`.

## Run locally
Open `index.html` in a browser, or run `python3 -m http.server` and visit http://localhost:8000.

## Structure
- `index.html` the whole site (HTML, CSS, JS, inline SVG logos)
- `assets/favicon.svg` site icon
- `404.html` custom not-found page
- `.nojekyll` tells GitHub Pages to serve files as-is

## Notes
- Only external resource: Google Fonts (Chakra Petch, JetBrains Mono), with system-font fallbacks.
- Logos are stylized inline SVGs. To use official logos, add them to `assets/` and swap the `<use href="#...">` references for `<img src="assets/...">`.
- All attack tests run only in isolated lab environments.
