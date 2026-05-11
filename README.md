# Delco City Limits

Static site for the Delco City Limits birthday fest — plain HTML/CSS, ready for [GitHub Pages](https://pages.github.com/).

## Local preview

From the repo root:

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080`.

## Deploy (GitHub Pages)

1. Push this repo to GitHub.
2. **Settings → Pages**: deploy from branch **`main`** (or `master`), folder **`/` (root)**.
3. Add your custom domain **`delcocitylimits.com`** in Pages settings. This repo includes a **`CNAME`** file with that hostname.
4. At Namecheap (or your DNS host), point the apex domain to GitHub Pages ([current A records](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain)). Optionally add a **`www`** CNAME if you use it.
5. Enable **Enforce HTTPS** once DNS validates.

## Fonts

Webfonts are loaded from `css/styles.css` via `@font-face`. Filenames are **case-sensitive** on GitHub Pages:

| File | Format | Family |
|------|--------|--------|
| `fonts/TAN-NIMBUS.woff2` | WOFF2 (primary) | TAN Nimbus |
| `fonts/TAN-NIMBUS.woff` | WOFF (fallback) | TAN Nimbus |
| `fonts/lazy_dog.ttf` | TrueType | Lazydog |
| `fonts/Hangyaboly.ttf` | TrueType | Hangyaboly |

If you replace any file, keep the same name or update the paths in `css/styles.css`. Confirm your license allows hosting font files in a public GitHub repository.

## Project layout

- `index.html` — Landing page (lineup, date, location). Poster asset optional in `assets/`.
- `set-times.html` — Schedule (placeholder times; edit as needed).
- `faq.html` — Logistics and starter FAQ copy.
- `css/styles.css` — Palette, typography, layout.
