# cheap proxies: what per-IP and per-GB pricing really costs, and how to buy residential IPs that don't expire

Most people searching for cheap proxies already have a quote in front of them. The problem usually isn't that the number is too high — it's that the number doesn't survive contact with month two. A $3/GB rate with a 10 GB monthly minimum costs $30 whether you scrape 10 GB or 400 MB. A $0.22/IP rate turns into $0.30/IP the moment you order 20 IPs instead of 10,000.

So "cheap" is really a question about billing structure. Divide providers into three price tags and the picture gets a lot clearer:

- **Per IP, per month** — predictable, but you pay for idle capacity
- **Per GB** — flexible, but rates swing 5x between the entry tier and the bulk tier
- **Per successful request** — the only number that matters in production, and the one nobody advertises

The third one is why a $1/GB provider can be more expensive than a $3/GB provider if it fails on your target and you have to retry.

## The three ways a cheap proxy quote quietly gets expensive

**1. Traffic that expires, or a minimum you can't shrink.** Monthly subscriptions built around a bandwidth allowance punish uneven workloads. If your project burns 80 GB in a busy week and 4 GB the next, you bought capacity you never used. Pay-as-you-go balances don't have that problem — but check the validity window, because "never expires" and "expires in 180 days" are very different products at the same rate.

**2. Headline rates that require volume.** Decodo's own writeup on budget ISP proxies makes the point bluntly: Webshare's $0.225/IP rate requires a 10,000-IP order, while the 20-IP package costs $0.30/IP. The same pattern shows up across the market. The advertised price is the price at scale, not the price you'll pay on day one.

**3. Free proxies.** Zero dollars, and there's a reason. ZDNET's 2026 buyer's guide recommends paid providers specifically because many free options monetize you instead — through data resale or worse. PCMag's proxy coverage makes the same argument, and adds that free pools are shared, logged, and unpredictable. If your traffic matters at all, free is the most expensive tier.

For context on where the market sits in 2026: premium residential bandwidth clusters around **$3–$8 per GB**, a budget tier sits under **$2 per GB**, and datacenter IPs are cheaper still. That's the backdrop for anything below.

## Where 9Proxy sits in that picture

9Proxy sells residential proxies only. Its official documentation describes two products: **Residential Proxy by IPs** (a fixed number of residential IPs with unlimited traffic while each IP is active) and **Residential Proxy by GB** (a bandwidth balance that generates unlimited endpoints). Bundles combine both. There's no monthly subscription — everything is a prepaid balance.

That distinction matters more than the sticker price. On the IP side, bandwidth is effectively unlimited, so heavy data transfer doesn't cost extra. Each residential IP stays alive somewhere between a few hours and roughly 24 hours. On the GB side, you're paying for traffic with unlimited endpoint generation, which suits rotation-heavy work where each request is light.

Two practical differences between the models, straight from the docs:

|  | Residential by IPs | Residential by GB |
| --- | --- | --- |
| Billing | Fixed package by IP count | Fixed package by GB |
| Validity | IPs never expire until used | 180 days (unlimited on Enterprise) |
| Traffic | Unlimited while active | Limited to purchased GB |
| IP lifetime | A few hours to ~24h | Rotates per request or per session |
| Setup | Requires the 9Proxy desktop app for local port forwarding | Works from the dashboard via user/pass or IP whitelist |

One thing worth flagging on prices: 9Proxy ran the first price adjustment in its history effective **June 1, 2026**, raising IP-based and bundle pricing while leaving GB-based packages untouched. Older pages still advertising "from $0.015/IP" reflect the pre-adjustment entry rate; the current published floor is roughly **$0.018/IP** at the largest tiers, and **$0.68/GB** at the top bandwidth tiers. If you're comparing against a review written before mid-2026, the IP numbers you're reading are probably stale.

### IP-based residential plans

These are the plans to look at if your work involves long sessions, account-based tasks, or data volumes that make per-GB math scary. Unlimited traffic per IP is the actual discount.

| Package | Rate per IP | Total | Billing |
| --- | --- | --- | --- |
| 100 IPs | $0.24 | **$24** | One-off, IPs don't expire · [ 100 IPs 套餐](https://bit.ly/9-Proxy) |
| 500 IPs | $0.144 | **$72** | One-off · [ 选择 500 IPs 方案](https://bit.ly/9-Proxy) |
| 1,000 IPs + 500 bonus | $0.084 | **$126** | One-off · [ 1,500 IPs 优惠包](https://bit.ly/9-Proxy) |
| 2,500 IPs | $0.084 | **$210** | One-off · [ 解锁 2,500 IPs 价格](https://bit.ly/9-Proxy) |
| 5,000 IPs | $0.072 | **$360** | One-off · [ 查看 5,000 IPs 套餐](https://bit.ly/9-Proxy) |
| 15,000 IPs | $0.048 | **$720** | One-off · [ 15,000 IPs 批量方案](https://bit.ly/9-Proxy) |
| 25,000 IPs | $0.035 | **$863** | One-off · [ 25,000 IPs 代理包](https://bit.ly/9-Proxy) |
| 50,000 IPs | $0.029 | **$1,438** | One-off · [ 50,000 IPs 大额套餐](https://bit.ly/9-Proxy) |

High-volume business tiers, for teams buying in the hundreds of thousands:

| Package | Rate per IP | Total | Billing |
| --- | --- | --- | --- |
| 100,000 IPs | $0.023 | **$2,300** | One-off · [ 企业级 10 万 IPs](https://bit.ly/9-Proxy) |
| 200,000 IPs | $0.021 | **$4,140** | One-off · [ 20 万 IPs 方案](https://bit.ly/9-Proxy) |
| 500,000 IPs | $0.018 | **$8,625** | One-off · [ 50 万 IPs 报价](https://bit.ly/9-Proxy) |

### GB-based residential plans

Pay for traffic, generate as many endpoints as your balance allows. Rotation and sticky sessions are both supported; targeting covers country, state, city and ISP.

| Package | Rate per GB | Total | Validity | Billing |
| --- | --- | --- | --- | --- |
| 5 GB | $3.00 | **$15** | 180 days | One-off · [ 5 GB 试用包](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | $2.10 | **$105** | 180 days | One-off · [ 55 GB 流量包](https://bit.ly/9-Proxy) |
| 100 GB | $1.50 | **$150** | 180 days | One-off · [ 100 GB 流量套餐](https://bit.ly/9-Proxy) |
| 200 GB | $1.00 | **$200** | 180 days | One-off · [ 200 GB 方案](https://bit.ly/9-Proxy) |
| 1,000 GB | $0.80 | **$800** | 180 days | One-off · [ 1,000 GB 大流量包](https://bit.ly/9-Proxy) |
| 2,000 GB | $0.75 | **$1,500** | 180 days | One-off · [ 2,000 GB 流量方案](https://bit.ly/9-Proxy) |

Enterprise bandwidth, where the 180-day clock goes away:

| Package | Rate per GB | Total | Validity | Billing |
| --- | --- | --- | --- | --- |
| 3,000 GB | $0.72 | **$2,160** | Unlimited | One-off · [ 3,000 GB 长期套餐](https://bit.ly/9-Proxy) |
| 6,000 GB | $0.70 | **$4,200** | Unlimited | One-off · [ 6,000 GB 流量包](https://bit.ly/9-Proxy) |
| 10,000 GB | $0.68 | **$6,800** | Unlimited | One-off · [ 10,000 GB 企业方案](https://bit.ly/9-Proxy) |

### Bundle plans

Built for mixed workloads — some tasks need a stable IP, others need traffic.

| Bundle | Package | Price | Billing |
| --- | --- | --- | --- |
| Starter | 100 IPs + 5 GB | **$30** | One-off · [ Starter 组合包](https://bit.ly/9-Proxy) |
| Popular | 1,500 IPs + 50 GB | **$180** | One-off · [ Popular 组合套餐](https://bit.ly/9-Proxy) |
| Pro | 5,000 IPs + 500 GB | **$720** | One-off · [ Pro 组合方案](https://bit.ly/9-Proxy) |

## Which structure is actually cheaper for your workload

Here's the part the pricing pages won't do for you. Take a project that moves about 100 GB.

- Buying it as bandwidth: **$150** on the 100 GB tier.
- Buying it as IPs: **$24** for 100 IPs, with unlimited traffic.

That gap is the whole argument for IP-based plans — if your architecture can spread the work across 100 IPs and keep each session short enough to fit inside a residential IP's lifespan. Where it falls apart is burstiness. Residential IPs live a few hours to a day, so a job that needs 100 concurrent clean IPs *right now* burns inventory fast, and you'll be topping up. Bandwidth plans don't care about that; they rotate through the full pool on demand.

A rough sorting rule:

- **Steady, session-heavy, unpredictable data volume** → IP-based. Multi-account management, long-running scraping, anything where "it stopped because I ran out of gigs" would be a catastrophe.
- **Bursty, rotation-heavy, light per request** → GB-based. SERP monitoring, price checks, ad verification, geo-testing.
- **Both on the same account** → a bundle, since buying the pieces separately usually costs more.

## Cutting the balance further

A few things genuinely reduce what you pay, in rough order of how much they matter:

**Reuse yesterday's IPs.** 9Proxy's "Today List" feature lets you reuse IPs issued in the last 24 hours without paying again. Third-party reviews put the saving at up to 30% on recurring daily tasks — that's the single biggest lever if your work is repetitive rather than one-shot. The vendor also documents a 60-second automatic replacement policy for IPs that fail.

**Check your payment method.** Selected payment methods have carried an extra **5% discount or 5% product bonus**. It's applied at checkout, not advertised on the plan grid.

**Use a referral link.** 9Proxy's partner program advertises a **5% discount for referred users**, which is what an invite-based signup carries — you'll see it on your first order when you [👉 注册 9Proxy 账户并领取推荐优惠](https://bit.ly/9-Proxy).

**Watch the seasonal campaigns — and check the expiry dates.** The Lunar New Year campaign ran a code worth **8% off** regular IP and GB packages between January 23 and February 23, 2026. April 2026 had a **9% back** offer: your first paid GB order of the month generated a single-use coupon (format `X9_[number]`) that appeared under Dashboard → My Account → My Coupons and applied automatically at checkout. That coupon expired **June 30, 2026**, and it never applied to bundle or IP-based orders. Both campaigns are finished, so treat them as evidence of how the promo cycle works rather than something to claim at checkout today — current offers live in the dashboard's coupon section.

Payments cover cards, crypto (USDT, BTC, ETH, LTC, DOGE among others), Alipay, Apple Pay and Google Pay, which matters if you're outside card-friendly jurisdictions.

## What you give up at this price point

None of the above is free money, and pretending otherwise would be a disservice.

- **Pool size.** 9Proxy advertises 20M+ residential IPs across 90+ countries. The enterprise incumbents advertise 100M+ and up. That gap shows up on narrow targets and Tier 3 geographies, where the budget tier's success rate drops faster than the premium tier's.
- **No mobile proxies.** The lineup is residential, full stop. Datacenter proxies have been listed as "coming soon" by resellers but aren't part of the current documented product set.
- **Windows dependency on the IP model.** The IP-based product routes traffic through the 9Proxy desktop app. If your stack runs headless on Linux, the GB model is the practical path, since it works directly from the dashboard with user/pass or IP whitelisting.
- **Streaming is not the use case.** One third-party review found major streaming platforms frequently blocked 9Proxy's IPs. For unblocking Netflix, use a VPN, not a residential proxy pool.
- **City-level targeting is narrower than premium providers.** The docs list country, state, city and ISP targeting; a 2026 cost comparison still rated its city granularity as limited next to the top-tier names.
- **Trials are limited.** There's no free tier published on the pricing page. Representatives have said limited trials are offered to new users subject to availability, and at least one directory lists a $0.02 one-off paid trial. Don't plan around a free trial you haven't confirmed — the smallest paid entry point is **$15** for 5 GB or **$24** for 100 IPs, and both are low-risk enough to test with.

## FAQ

**Are cheap proxies safe to use?**
Cheap *paid* is a fundamentally different product from free. Free pools are shared, often logged, and commonly monetized by reselling your traffic. A $24 IP package from a provider that documents its network is not the same risk category.

**Do 9Proxy balances expire?**
IP-based packages: no. Those IPs stay in your account until used. GB-based: 180 days of validity, except the 3,000 / 6,000 / 10,000 GB Enterprise tiers, which have unlimited validity.

**Is there a monthly subscription?**
No. Everything is a prepaid balance with volume-based discounts. There's no rebill, which is why buying before a price adjustment is a one-time decision rather than a temporary discount.

**Do I need to buy IPs and bandwidth separately?**
No — the bundle plans exist precisely for that, and they're cheaper than the two components bought separately.

**What protocols are supported?**
HTTP/HTTPS and SOCKS5, with SOCKS5 supported natively, including for anti-detect browsers and custom scripts.

## The short version

If you're shopping on price alone, the number that matters isn't the $/GB on the landing page — it's whether the billing structure matches how your workload actually consumes capacity. Unlimited-bandwidth IP packages at $24 for 100 IPs are the cheapest route for session-based work. Bandwidth packages from $3/GB down to $0.75/GB fit rotation-heavy jobs. And the thing that has historically made 9Proxy cheap isn't a discount code at all: it's that nothing rebills and nothing gets thrown away at the end of a month.

If that matches the shape of your project, [👉 在 9Proxy 领取当前最低价 IP 与流量套餐](https://bit.ly/9-Proxy) and start at the smallest tier. Test the success rate on your own targets before you buy 15,000 IPs on someone else's benchmark.
