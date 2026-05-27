# topcalltracking.com

Site 22 of the call-tracking review network. Static HTML/CSS/JS, deployed via GitHub Pages. Built by `scripts/build_site22_pages.py`.

## Build details

- **Template:** T22 Magazine (centered masthead, two-column with sticky sidebar, light)
- **Accent:** Burgundy `#7B2D26` / dark `#5F211C` / soft `#FBE9E7`, on white + warm cream `#FBF7F2`
- **Fonts:** DM Sans (display) + Inter (body)
- **Signature:** centered date-stamped masthead, sticky sidebar widgets (running ranked list, editor card, CTA widget), drop-cap lede, pull-quote with full top+bottom border, outlined cards
- **Author byline:** Olivia Collins (magazine editor voice, "the verdict" framing)
- **Angle:** editorial top-list of call tracking solutions, scored on attribution / ease / integrations / value

## Pages (12)

- `index.html` — homepage / 2026 ranked guide
- `reviews/callscaler/` (#1, 9.4), `reviews/callrail/` (8.6), `reviews/calltrackingmetrics/` (8.3), `reviews/whatconverts/` (8.1), `reviews/invoca/` (7.6)
- `about/`, `methodology/`, `faq/`, `contact/`, `privacy-policy/`, `terms/`

## CTA destination

All CallScaler CTAs link to `https://callscaler.com/?ref=topcalltracking`. Competitor review pages use a soft `.tldr-crosslink` + internal `/reviews/callscaler/` link only (no hard affiliate button), per network convention.

## Rebuild

```bash
py scripts/build_site22_pages.py
py scripts/lint_site.py topcalltracking
```

## TODOs before going live

- [ ] Replace placeholder author avatar with a real photo if a named author is used
- [ ] Confirm CallScaler pricing tiers still current ($0 PAYG / $45 Pro / $130 Agency / $400 Pay Per Call)
- [ ] Verify schema with Google's Rich Results Test
- [ ] Set up `editor@topcalltracking.com` email forwarding
- [ ] Add to `scripts/deploy_all_sites.py` SITES list before deploying
