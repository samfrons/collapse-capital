# Collapse Capital

**Positioned Since the Pleistocene.**

A satirical wealth-management prospectus that reports real climate and
economic collapse data as bullish market signals. Every figure is sourced
(NOAA, NASA GISS, NSIDC, IEA, Stanford AI Index, Epoch AI, SEC filings,
corporate environmental reports) — the only invention is the voice that
finds it encouraging.

Flip the **Investor ⇄ Human** toggle to read the same data two ways: as a
fund's pitch deck, or as what it actually describes.

> This is satire. The data, unfortunately, is not. Collapse Capital is not a
> fund, holds no positions, and manages nothing but a point.

## Live site

Deployed on Vercel: **https://collapse-capital.vercel.app**

## Pages

- `index.html` — the prospectus.
- `collapse-tech.html` — **Threshold**, the research arm: an interactive
  atlas of Earth's tipping points, plus the underfunded climate
  technologies worth funding before they tip. Linked from the prospectus'
  nav and its closing section.

## Tech

Two self-contained static pages. No framework, no build step. Fonts load
from Google Fonts; charts, icons, and animation are hand-rolled inline
SVG/CSS/JS. Threshold's globe additionally uses D3 + TopoJSON (via CDN)
for its four view modes (emissions, satellite, night, atlas).

## Local preview

Any static file server works, e.g.:

```bash
npx serve .
# or
python3 -m http.server 8000
```

Then open the printed localhost URL.

## Deploy

Deployed via the [Vercel CLI](https://vercel.com/docs/cli) with zero config
(static site, no build command):

```bash
vercel        # preview deployment
vercel --prod # production deployment
```

## License

MIT — see [LICENSE](LICENSE). The satire is free to reuse; the underlying
data belongs to its original sources, cited in-page.
