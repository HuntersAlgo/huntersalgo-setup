# Changelog

Every shipped change, dated, with the reason. Post-mortems get the same treatment if a release later needs one.

I post every release in the [Discord](https://huntersalgo.com/discord) as it goes out, usually once or twice a month, and answer questions about it there.

Entries are newest first. Each one is tagged as a release, an improvement or infra.

## HunterStrike is out

*24 September 2026, release*

HunterStrike, the intraday levels indicator announced on 11 September, is now in the subscriber download.

Import it with the strategies (Tools, then Import, then NinjaScript Add-On), add it to a chart, and enter your Whop email when it asks. It is included in every plan at no extra charge.

- [HunterStrike](https://huntersalgo.com/indicators/hunterstrike)
- [Install guide](https://huntersalgo.com/guides/install-ninjatrader-strategy)

## Site clean-up: indicators in the footer, honest report pages, faster images

*12 September 2026, improvement*

- The footer now links every section rather than ten pages, so /indicators, /changelog, /glossary and /refer stop being reachable only through the header.
- The eleven per-strategy report pages that have no data yet are marked noindex and dropped from the sitemap. They stay readable, but Google is no longer asked to index eleven near-identical placeholders.
- Six report pages had the strategy's full SEO title in their heading. They use the short name now.
- Images under /public were revalidating on every page view and now cache for a month.
- HunterML and HunterStrike gained product schema, and the homepage FAQ is finally marked up as one.

Links:

- [Results](https://huntersalgo.com/results)
- [Indicators](https://huntersalgo.com/indicators)

## Retired the Daily Market Brief

*11 September 2026, infra*

The weekday 11:30 UTC brief is gone: the cron trigger, the digest route and the site copy that promised it.

Subscriber records were kept, so nobody has to re-subscribe if a future email ever replaces it. The free-guide landing page followed on 12 September and now redirects to the guides library.

- [Guides](https://huntersalgo.com/guides)

## HunterStrike: the day's levels, drawn before the open

*11 September 2026, release*

HunterStrike is a NinjaTrader 8 indicator that sets nine intraday levels from the New York pre-market, holds them for the session, and puts an arrow on every bar that closes through one. Wicks do not count.

It draws and marks. It places no orders.

The one decision is Normal or Flipped. The level maths is fixed so every subscriber reads the same lines, while colours and visibility are yours.

It is included in every plan on the same licence email, at no extra charge. It ships in the next package update and appears in your indicator list once you install it.

- [HunterStrike](https://huntersalgo.com/indicators/hunterstrike)
- [Playbook](https://huntersalgo.com/indicators/hunterstrike/playbook)

## Agent readiness, DNSSEC, and a faster mobile homepage

*7 September 2026, infra*

- Published the machine-readable layer a retrieval agent needs: llms.txt, an AI catalogue at /.well-known/ai-catalog.json, an OpenAPI description, Content-Signal directives in robots.txt, and Markdown representations of the blog, guides and strategy pages under content negotiation.
- Enabled DNSSEC and published the agent discovery record.
- Merged the PageSpeed work, which moved about 200 KB of inlined CSS out of every uncached HTML response into cached external stylesheets.

Links:

- [Methodology](https://huntersalgo.com/methodology)

## Aligned site copy to Whop storefront

*5 May 2026, improvement*

Synced the site to the live Whop storefront:

- The trial duration is 3 days, corrected from 5.
- A card is required at Whop signup.
- All sales after the trial are final under Whop's terms. This replaces the earlier 14-day critical-fault refund clause.
- The Whop review count shown on the site was brought up to date.
- The sale running at the time was surfaced as a countdown banner on the pricing page.

Links:

- [Pricing](https://huntersalgo.com/pricing)
- [Refund policy](https://huntersalgo.com/refund-policy)
- [Reviews](https://huntersalgo.com/reviews)

## Analytics, schema, and AI-search readiness

*26 April 2026, infra*

- Unblocked Cloudflare Insights and the GA4/GTM analytics scaffolding (a CSP fix).
- Added Product/AggregateOffer/AggregateRating, ItemList, Dataset, TechArticle, ContactPage, Blog and CollectionPage JSON-LD across priority pages.
- Rewrote robots.txt to allow AI search retrieval bots (OAI-SearchBot, Claude-SearchBot, PerplexityBot) while keeping training crawlers out.

Links:

- [Methodology](https://huntersalgo.com/methodology)
- [Results](https://huntersalgo.com/results)

## Site-wide trust and conversion overhaul

*26 April 2026, improvement*

- Surfaced the trial mechanic at the moment of the click across the homepage and pricing page.
- Added an honest backtest-status column to /results, so the five strategies still in development read as such.
- Added env-driven Discord and Whop review counters so trust stats do not drift from reality.

Links:

- [Pricing](https://huntersalgo.com/pricing)
- [Refund policy](https://huntersalgo.com/refund-policy)
- [Discord](https://huntersalgo.com/discord)

---

Mirrored from huntersalgo.com on 30 September 2026. The site is the canonical version.
