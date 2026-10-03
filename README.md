# Codex Echo Systems

Production website for **Codex Echo Systems LLC (CES)**.

| Item | Value |
|------|--------|
| Production website | https://codexechosystems.com |
| Repository | [mcgovernafi-blip/codexechosystems-web](https://github.com/mcgovernafi-blip/codexechosystems-web) |
| Deployment | GitHub Pages |
| Custom production domain | `codexechosystems.com` |
| HTTPS | Enabled (GitHub Pages certificate; Enforce HTTPS) |

This repository is the source of the live corporate site. It does not include paid services, tracking, advertising, or product sales.

## Pages

- `index.html` — company identity and concise statement
- `about.html` — company purpose
- `contact.html` — business email (`developer@codexechosystems.com`)
- `privacy.html` — privacy information
- `404.html` — custom not-found page for GitHub Pages
- `CNAME` — GitHub Pages custom domain (`codexechosystems.com`)
- `css/styles.css` — shared responsive styling
- `assets/` — approved CES brand marks and favicon

## Local preview

From the repository root:

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000` in a browser. Local preview is for development only; production is served at https://codexechosystems.com.

## Deployment notes

- Publish from the default branch via GitHub Pages.
- Keep `CNAME` contents exactly: `codexechosystems.com`
- Do not assume a `*.github.io/codexechosystems-web` base path.
- CES email DNS (MX/SPF/DKIM/DMARC) is managed outside this repository and must not be changed here.
