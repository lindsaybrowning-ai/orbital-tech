# VP Sales Panel: Orbital

A single-page static site (one `index.html`, no build step). Tabs: Overview, Section 1, Section 2, Leadership, Orbital math, Orbital ICP.

## Files

- `index.html`: the whole site (HTML, CSS and JavaScript in one file; fonts load from Google Fonts)
- `vercel.json`: security headers and a `noindex` header so search engines skip the site
- `robots.txt`: asks crawlers not to index anything
- `.gitignore`

## Put it on GitHub

```bash
cd orbital-vp-sales-panel
git init -b main
git add .
git commit -m "Initial commit"
# create an empty PRIVATE repo on GitHub first, then:
git remote add origin git@github.com:<your-username>/orbital-vp-sales-panel.git
git push -u origin main
```

## Host it on Vercel

1. In Vercel, choose **Add New > Project** and import the GitHub repo.
2. Framework Preset: **Other**. Leave Build Command, Output Directory and Install Command empty.
3. Click **Deploy**. Every push to `main` redeploys.

## Notes

- `noindex` stops search engines, but anyone with the link can open the page. The page holds interview prep, so keep the repo private and check Vercel's deployment protection options for your plan before sharing the link widely.
- To change content, edit `index.html`, commit and push.
- Preview locally: `python3 -m http.server 8000`, then open http://localhost:8000
