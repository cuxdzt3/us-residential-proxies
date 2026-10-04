# us residential proxies: how to pick city-level US IPs for scraping, SEO and ad checks without overpaying

Shopping for US residential proxies goes sideways fast, and it's almost always for the same reason: providers advertise a global number — 90 million IPs, 195 countries — and say nothing useful about how deep the American pool actually goes. That country-level number can hide the fact that your target city has four exits and three of them are already burned.

Then there's the billing question. Per gigabyte or per IP? The answer depends on whether your job is bandwidth-hungry or session-hungry, and picking the wrong model is the difference between a $30 test and a $600 habit.

Below is the buying process that actually matters, with 9Proxy's current plan lineup as the worked example — because it's one of the few providers that publishes both billing models side by side, and its US targeting goes down to state, city, ZIP and ISP.

## What US residential proxies actually solve

A residential IP is borrowed from a real home connection, so it carries the reputation of a real household in a real market. For US work, that reputation is the point. American sites are aggressive about two things: datacenter ranges (blocked on sight at the IP layer) and non-US traffic (served different prices, different inventory, sometimes a straight redirect).

Two concrete things follow from that:

**Location-accurate data.** Google results, Amazon pricing, delivery estimates, state tax display and retail stock all vary by where the request appears to come from. A US exit in the wrong state gives you a plausible-looking answer that's quietly wrong.

**Fewer blocks.** Clean residential IPs pass reputation checks that datacenter and reused proxy ranges fail. If you've ever watched a scraper work perfectly for two days and then return challenge pages forever, that's usually IP reputation, not your code.

What they don't solve: heaviest-protection targets at high frequency. Amazon, LinkedIn and Google SERPs at real volume still punish budget-tier pools, and every provider's price tier maps roughly to that reality. Third-party price roundups published in 2026 put budget residential at roughly $0.70–$2 per GB, mid-market around $3–$5, and Bright Data or Oxylabs in the $8–$11 range. Cheaper pools simply have fewer tricks.

## Decide how much targeting precision you need

This is the step most buyers skip, and it's the one that determines your bill. Nine times out of ten, people over-buy precision.

| Your actual job | Precision you need | Session style |
| --- | --- | --- |
| National catalog monitoring, bulk SERP pulls | Country (US) | Rotate per request |
| State-level price or availability checks | State | One bounded session per market |
| Local SEO, local pack tracking | City | Consistent per observation |
| Ad verification in a specific DMA | City or ZIP | Consistent per observation |
| Matching a carrier or ISP fingerprint | ISP / ASN | Sticky |
| Long-running account work | City or state | Sticky, hours at a time |

9Proxy's dashboard supports country, state, city, ZIP and ISP targeting on its bandwidth-based plans, and both rotating and sticky sessions. Its changelog describes the setup plainly: pick the auth method, pick the location filter, choose sticky or rotating, generate endpoints, export `.txt` or `.csv`. Sticky keeps the same IP for a set number of minutes; rotating hands you a fresh one per request or per session.

Worth saying out loud: ZIP-level precision is not the same as ZIP-level inventory. Every provider's per-city stock shifts daily as home devices come online and drop off. Buy precision you'll use, then measure whether the exits you get actually match what you asked for.

## Per-GB vs per-IP: the math that decides your plan

The two billing models reward opposite workloads.

**Per-GB** charges for traffic. It wins when each request is small and you rotate constantly — geo-checks, price snapshots, ad verification, API polling. You can burn through thousands of IPs without paying for the privilege of holding them.

**Per-IP with unlimited bandwidth** charges for addresses. It wins when your traffic is heavy or unpredictable — full browser sessions, long scraping runs, account work where you keep the same identity for hours. Ten requests or ten thousand through the same IP costs the same.

A rough sanity check: if your average response is a 40–80 KB JSON or HTML payload, you'll get a lot of mileage out of 10 GB. If you're rendering JavaScript-heavy pages, each page can be 2–5 MB and a per-GB bill climbs fast. One reviewer who pushed roughly 12 million requests through 9Proxy in a month-long test noted that on the IP-based side the gigabyte counter never became a consideration at all. That's the whole argument for per-IP pricing.

👉 [Compare the per-GB and per-IP packages directly on your own workload](https://bit.ly/9-Proxy)

## 9Proxy's full plan lineup and current prices

9Proxy sells three product families: IP-based packages with unlimited bandwidth, GB-based packages, and bundles that combine both. It announced a price adjustment for the IP-based and bundle packages effective June 1, 2026 — the first in the company's three-year history, by its own account. GB-based pricing was left untouched. The figures below reflect the post-adjustment rates.

### IP-based packages (unlimited bandwidth per IP, IPs don't expire)

| Package | IPs you receive | Price | Effective cost per IP | Buy |
| --- | --- | --- | --- | --- |
| 100 IPs | 100 | $24 one-time | ~$0.24 | [Start with 100 US IPs](https://bit.ly/9-Proxy) |
| 500 IPs | 500 | $72 one-time | ~$0.14 | [Get the 500-IP package](https://bit.ly/9-Proxy) |
| 1,000 IPs + 500 bonus | 1,500 | $126 one-time | ~$0.084 | [Take the 1,000 + 500 IP tier](https://bit.ly/9-Proxy) |
| Mid-volume tiers (2,500–50,000 IPs) | 2,500–50,000 | Stepped per-IP pricing between the entry tiers and wholesale rates | Scales toward ~$0.03 | [Request a mid-volume US package](https://bit.ly/9-Proxy) |
| 100,000 IPs | 100,000 | $2,300 one-time | ~$0.023 | [Price the 100,000-IP inventory](https://bit.ly/9-Proxy) |
| 500,000 IPs | 500,000 | $8,625 one-time | ~$0.017 | [Enquire about 500,000 IPs](https://bit.ly/9-Proxy) |

The system is balance-based. You top up and draw IPs from the balance, so buying before a price change locks the rate.

### GB-based packages (pay for traffic, not addresses)

| Package | Price per GB | Total | Validity | Buy |
| --- | --- | --- | --- | --- |
| 5 GB | $3.00 | $15 | 180 days | [Try 5 GB of US residential traffic](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | $2.10 | $105 | 180 days | [Buy the 50 + 5 GB pack](https://bit.ly/9-Proxy) |
| 100 GB | $1.50 | $150 | 180 days | [Get 100 GB](https://bit.ly/9-Proxy) |
| 200 GB | $1.00 | $200 | 180 days | [Get 200 GB](https://bit.ly/9-Proxy) |
| 1,000 GB | $0.80 | $800 | 180 days | [Scale to 1,000 GB](https://bit.ly/9-Proxy) |
| 2,000 GB | $0.75 | $1,500 | 180 days | [Scale to 2,000 GB](https://bit.ly/9-Proxy) |
| 3,000 GB (Enterprise) | $0.72 | $2,160 | No expiry | [Compare Enterprise GB tiers](https://bit.ly/9-Proxy) |
| 6,000 GB (Enterprise) | $0.70 | $4,200 | No expiry | [Compare Enterprise GB tiers](https://bit.ly/9-Proxy) |
| 10,000 GB (Enterprise) | $0.68 | $6,800 | No expiry | [Compare Enterprise GB tiers](https://bit.ly/9-Proxy) |

Enterprise also changes what the account can do, not just the rate: unlimited data validity, one owner plus up to five team members, shared bandwidth that doesn't expire inside the team, per-member traffic limits, activity logs and unlimited share codes.

### Bundle packages (IPs plus traffic in one purchase)

| Bundle | What's inside | Price | Buy |
| --- | --- | --- | --- |
| Starter | 100 IPs + 5 GB | $30 | [Get the Starter bundle](https://bit.ly/9-Proxy) |
| Growth | 1,500 IPs + 50 GB | $180 | [Get the Growth bundle](https://bit.ly/9-Proxy) |
| Pro | 5,000 IPs + 500 GB | $720 | [Get the Pro bundle](https://bit.ly/9-Proxy) |

Bundled traffic carries a 180-day validity window. If your work is mixed — some sticky account sessions plus some burst rotation — a bundle costs less than buying the two halves separately.

One caveat worth stating plainly: 9Proxy's pricing page routes some of the larger tiers toward a sales conversation, and promos rotate. Check the live figure before you commit to a volume number.

## Features that matter when you're running US traffic

The plan buys you addresses. These are the things that decide whether a US campaign is manageable at 3 a.m.

**Auto-refresh.** Offline IPs get detected and replaced automatically, so a long scrape doesn't die because a home connection in Ohio went to sleep. The company says replacements happen within 60 seconds of a failed connection.

**Auto-rotation.** Set an interval and proxies cycle on schedule — useful on platforms that get jumpy when one IP hammers them.

**Today List.** Any proxy you used in the last 24 hours can be reused free if it comes back online. 9Proxy estimates that trims 20–30% off repeat workloads, and for a daily price-monitoring job that's not a rounding error.

**Contact points for real work.** HTTP/HTTPS and SOCKS5, so antidetect browsers, Scrapy, Puppeteer and Python's requests library all connect without protocol conversion. Username/password auth or IP whitelisting. A Windows/Mac desktop client, a zero-install browser option, a mobile device tool, and a public API for pipelines that need session control from code.

**Payments.** Cards, bank cards, Alipay, Apple Pay, Google Pay and crypto (USDT, BTC, ETH, LTC, DOGE and others). 9Proxy advertises a 5% bonus in extra IPs for crypto payments.

## Where 9Proxy fits — and where it doesn't

The honest read is that 9Proxy is a budget-tier provider that behaves like a slightly better one. Reviews in 2026 consistently land in the 4.3–4.8 out of 5 range from aggregators, and one month-long third-party test reported roughly a 99.5% success rate at about 0.6 seconds average response — numbers in line with what the company advertises (99.95% uptime, 20M+ IPs across 90+ countries).

Choose it when:

- Your US targets sit in the light-to-moderately protected range: retail catalogs, marketplaces, travel and real-estate listings, regional news, public records.
- Bandwidth is unpredictable or heavy, so per-IP unlimited data kills your cost anxiety.
- You want state, city, ZIP or ISP targeting without enterprise pricing.
- You're running account work in antidetect browsers and need clean, separated IPs at a per-address price.

Look elsewhere when:

- You need Amazon, Google or LinkedIn at serious volume. That's the tier where the $8–$11/GB providers earn their price, and 9Proxy's pool and tooling aren't built for it.
- You need a 100M+ IP network. 9Proxy's 20M+ is deliberately smaller, positioned as cleaner rather than bigger.
- Streaming unblocking is the goal. Third-party testing reported detection on services like Netflix — residential IPs are not a streaming tool, and most providers will tell you the same privately.
- You need polished, beginner-friendly onboarding. Multiple reviewers flag the workflow as technical: real residential IPs last a few hours and up to a day by nature, and you're expected to understand rotation, sticky sessions and auth.
- You want a guaranteed free tier. Trials exist but are limited and request-based, subject to availability. Ask support before assuming.
- Your use case involves high-abuse activity. At least one review notes 9Proxy enforces terms against things like sneaker copping and gaming to protect pool cleanliness, so read the terms before building a workflow around it.

It's also fair to note the network isn't spotless. One user report published in 2026 described the service going offline for about a week; a reseller listing on the same topic now states the IP network was restored and is operational. Worth knowing if uptime is a hard requirement for you.

## Setting up your first US proxy, step by step

1. **Create the account.** Sign up through the link below, pick a package, and keep your email clean — a dedicated address makes support tickets easier later.
2. **Choose the billing family you actually need.** Bursty rotation → GB. Heavy sessions or account work → IP-based. Both → bundle.
3. **Pick your auth method.** Username/password for cloud tools and multi-client setups; IP whitelisting if you'd rather skip credentials on a fixed server.
4. **Set location.** Select United States, then narrow to the state, city, ZIP or ISP your target actually serves.
5. **Choose session mode.** Rotating for scraping breadth, sticky when a task spans multiple steps.
6. **Generate and export.** Pull endpoints in your format of choice — `.txt` or `.csv` — or wire the API into your code.
7. **Test one connection first.** Hit a page that echoes your exit IP and confirm the city matches your intent before scaling to fifty ports.
8. **Add pacing.** Keep at least ~30 seconds between hits on the same IP for account work, and one IP per profile when you're separating identities.

## Which plan should you actually buy?

For a first US project, 5 GB at $15 is the cheapest way to find out whether 9Proxy's American exits behave on your targets — and switching to a bigger tier later costs you nothing but the difference.

If you already know your job is sticky and heavy, the 100-IP package at $24 with unlimited bandwidth is hard to argue with, and the 1,000 + 500 bonus tier at $126 drops the effective rate to under nine cents per IP. Agencies managing multiple client accounts usually start at the Growth bundle; anyone running daily US-wide monitoring at volume should price the 200 GB–1,000 GB range instead.

👉 [Open a 9Proxy account and pick your US package](https://bit.ly/9-Proxy)

## FAQ

### Are US residential proxies necessary for scraping American sites?

Not universally. Sites with light protection will serve datacenter IPs fine. As soon as you hit reputation checks or geo-restricted content — marketplaces, travel pricing, local SERPs, ad placements — residential IPs from the target market stop being optional.

### How long does a 9Proxy US IP stay alive?

Residential IPs are home connections, so they come and go. 9Proxy lists typical lifetimes from a few hours up to 24 hours, and its auto-refresh replaces dead ones. The 60-second replacement policy covers IPs that fail immediately.

### Can I target a specific US state or city?

Yes. Country, state, city, ZIP and ISP targeting are available on the bandwidth-based plans through the dashboard's proxy generator. Inventory depth per city varies by provider in this category, so test your specific market before committing to volume.

### Do the plans expire?

IP-based packages don't expire — the blog announcement on the June 2026 adjustment specifically says purchased IPs are held at the current rate and never expire. GB-based plans carry 180-day validity, except Enterprise bandwidth, which doesn't expire at all.

### Can I use 9Proxy with antidetect browsers?

Yes. SOCKS5 and HTTP/HTTPS are supported, and reviewers report it working with tools like Multilogin, Dolphin Anty and AdsPower. One IP per browser profile is the standard setup for keeping accounts unlinked.

### Is there a free trial?

Trials exist but are limited and granted on request, depending on availability — you'll need to tell support whether you want a trial measured in IPs or in GB.

## The short version

US residential proxies are a precision purchase, not a volume purchase. Work out whether your job needs country, state or city accuracy first, then decide between per-GB billing for rotation-heavy scraping and per-IP billing for bandwidth-heavy sessions. If your targets are in the light-to-moderate protection band and you'd rather not pay $8 a gigabyte, 9Proxy's $15 entry point and $24 unlimited-bandwidth IP package are cheap enough to test against your own target list — which is the only benchmark that matters anyway.
