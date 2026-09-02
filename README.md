# DEKA Building Group — website

Single-page site for DEKA Building Group Pty Ltd (Adelaide, SA).
Plain HTML, no build step, no dependencies.

## Files

| File | What it is |
|---|---|
| `index.html` | The entire site — markup and CSS in one file |
| `img/` | Project photography, logo (taupe + cream), favicon |
| `robots.txt` | Allows search engines, points at the sitemap |
| `sitemap.xml` | Single-page sitemap for Google Search Console |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Publishing with GitHub Pages

1. **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)** → **Save**

Live within a minute or two at `https://dmitriikap.github.io/DEKA/`.

### Custom domain (dekabuildingroup.com)

1. **Settings → Pages → Custom domain** → enter `dekabuildingroup.com` → Save.
   This creates a `CNAME` file in the repo.
2. At the registrar (currently Squarespace), replace the existing records with:

   | Type | Host | Value |
   |---|---|---|
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |
   | CNAME | www | dmitriikap.github.io |

3. Back in Settings → Pages, tick **Enforce HTTPS** once the certificate issues
   (can take up to an hour).

## Editing

Text and colours are all in `index.html`. The palette lives in the `:root` block
at the top as CSS custom properties — change a value there and it updates everywhere.

To swap or add a photo: drop the file in `img/`, then update the `src` and the
`<figcaption>` in the `#work` section.

## Brand

- Logo taupe `#97826F` (sampled from the artwork)
- Ground `#F2EFE9` · Dark `#332B24` · Accent `#6F5D4C`
- Type: Archivo (display), IBM Plex Sans (body), IBM Plex Mono (data), via Google Fonts

## Company

DEKA Building Group Pty Ltd · ABN 85 697 675 504 · Builder's Licence BLD 359133
Adelaide, South Australia · 0466 453 212 · dmitrii@dekabuildingroup.com
