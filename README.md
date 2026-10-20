# Paywall Audit — GeoZilla

**Live:** https://bterzic123.github.io/geozilla-paywall-audit/

Five paywall ideas for GeoZilla, each backed by a finding from Adapty's State of Paywalls 2026, plus a clickable rebuild of the paywall and the moment after close in GeoZilla's own design. The prototype has a Today / Proposed switch and numbered pins for each report finding.

## The ideas

| # | Idea | Report anchor | Outcome range |
| :-- | :-- | :-- | :-- |
| 1 | Pre-select the yearly, and price every plan per week | 2.4 pre-selection (90% keep a pre-selected weekly, 46% an annual) · 3.3 per-week framing (4%) · 5.3 annual-forward layout | ARPU +25–40%, observed in winning A/B tests |
| 2 | Give closing the paywall a second chance (your Basic plan, 8,99 €/week) | 4.5 second-chance paywalls (4% of apps, 0.88× the main paywall, beats it in 45%) | ARPU +10–15%, based on Adapty data |
| 3 | Put the role they picked in the headline | 3.5 personalized headlines (2%) · 5.3 onboarding personalization | CR +8–17%, observed in winning A/B tests |
| 4 | Bring your 25 million users and 4.5 stars to the price | 3.1 social proof (27%) · 5.3 social proof on the paywall | CR +10–30%, observed in winning A/B tests |
| 5 | Give the paywall its own close button, after three seconds | 3.7 close-button delay (22% of apps, 3–5 s most common) · 5.3 delay before close | CR +8–15%, observed in winning A/B tests |

## Slice used

The report is App Store data (Oct 2025 – Sep 2026). Most of GeoZilla's revenue comes from Google Play, India first, so the audit compares how the paywall is set up, not its conversion or prices. Where the report splits a number by category, it uses Lifestyle, GeoZilla's App Store category.

## The report

State of Paywalls 2026: https://adapty.io/state-of-paywalls/?utm_source=paywall-audit&utm_medium=github-pages&utm_campaign=sop_2026&utm_content=geozilla

## Grounding

Every price comes from GeoZilla's own paywall (EUR storefront, October 2026): 44,99 € a quarter, 12,99 € a week, 69,99 € a year, and 8,99 € a week on the Basic tab under Other Plans. Per-week figures are arithmetic on those prices. The rating (4.5 from 51K ratings) is from the US App Store listing. "Join 25+ Million Happy Users", the role subtitles and the three quotes are from GeoZilla's own onboarding, quoted verbatim.

Impact ranges are observed lifts from winning A/B tests in State of Paywalls 2026 and Adapty's own data, not measured results for GeoZilla.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. Add `?for=<first name>` to change who the page addresses.
