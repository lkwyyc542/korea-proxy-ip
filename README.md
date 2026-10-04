# south korea proxy: how to get a real Korean IP for Naver, Coupang and the sites that block foreign traffic

Korean sites don't just prefer local visitors, several of them require them. Naver returns different results to a foreign IP, and Naver Blog, Naver Cafe and Naver Shopping restrict or alter content for non-Korean visitors. Coupang prices and stock are set for the domestic market. Korean game platforms and sneaker releases check IP reputation before they check anything else.

So the useful question isn't "which provider sells a South Korea proxy." Plenty list the country. The useful question is whether the Korean IP you get will hold a session long enough to log in somewhere, whether the plan you're paying for makes sense for Korean traffic patterns, and what it costs per month to keep that running.

## Three different things get sold as a "Korea proxy"

The country label is the least important part of the decision. What matters is the address type, because Korean platforms treat the three types very differently.

**Residential rotating** — exits from real consumer connections, billed per gigabyte, IP changes per request or per session. This is the default working tool for Naver SERP scraping, Coupang monitoring and ad verification. Market pricing for Korea-capable residential traffic runs from roughly $1.75/GB on budget networks up to $4–$8/GB at the large enterprise vendors.

**Static residential / ISP** — one address that never changes, usually billed per day. Worth it when you're staying logged into a Korean account rather than collecting at volume. Expect around $3.90/day at the providers that sell it that way.

**Mobile / LTE** — carrier-grade addresses from Korean telcos. The most trusted and the most expensive, often around $2 per IP. Reach for it only when residential has already failed.

Rotating datacenter IPs cost about a dollar per gigabyte and get blocked by anything that matters in Korea. Free Korean proxy lists are worse than useless: unstable exits, high detection rates, and a steady history of traffic being harvested or injected. If a page loads through a free Korean IP, that's coincidence, not capability.

A snapshot of how the paid types compare for Korean work:

| Address type | Typical market price | Where it fails |
| --- | --- | --- |
| Rotating residential | $1.75–$8 / GB | Unstable under heavy login use |
| Static residential (ISP) | ~$3.90 / day | Small address pool, overkill for scraping |
| Mobile / LTE | ~$2 / IP | Priciest per GB, limited stock |
| Datacenter | ~$1 / GB | Detected fast on Korean platforms |

## What to check before you pay anyone

**Does the Korean exit exist on the endpoint you'll actually use?** This trips people up more than it should. Several providers offer Korea on the global gateway but not on their Korea-specific entrance ports, which changes how sticky sessions behave. Confirm the exact hostname and port you'll be sending traffic to, not the country list on the marketing page.

**How long does a session hold?** Rotating is fine for scraping. It's useless for anything that requires a persistent login. Korean platforms are aggressive about re-verification when an address changes mid-session, and while city-level targeting exists at most providers, some of them exclude it from the Korea ports. Ask for the sticky interval in minutes, not "configurable."

**Per gigabyte or per IP?** This one matters for Korea specifically. Korean pages are media-heavy — a Coupang listing with product images and reviews can be 250 KB or more. If you're browsing, maintaining sessions or pulling rich pages, metered bandwidth gets expensive fast, and a per-IP plan with unlimited traffic usually wins. If your job is high-volume, low-payload request firing, metered wins.

**How narrow can you filter?** Country-level targeting is enough for rank tracking. Price checks and delivery estimates that shift between metros need city or ZIP. Narrowing too far shrinks the available pool, so the honest setup is the loosenest filter that still answers your question.

**Protocol support.** HTTP(S) and SOCKS5 both, or you'll be rewriting integrations later.

## Where 9Proxy fits into Korean work

9Proxy is a residential proxy network advertising 20M+ IPs across 90+ countries, with South Korea among the supported locations and targeting that extends past country level into state, city, ZIP code and ISP. It speaks HTTP(S) and SOCKS5, and it sells two very different usage models rather than one subscription.

The reason that's relevant to Korea specifically: the per-IP model charges a fixed amount per address with unlimited bandwidth, while the per-GB model charges by traffic and gives you unlimited rotating endpoints. Paying per IP with no traffic ceiling removes the cost anxiety of loading heavy Korean pages, which is the opposite of how most Korea-capable residential providers price.

Single IPs start around $0.018, and bandwidth drops to $0.68/GB at the top tier. Both numbers undercut what the big enterprise vendors list for Korean residential traffic, and the trade-off is real: it's a shared global pool rather than a Korea-specialised network with carrier-level ASN guarantees.

Signing up through an invite code attaches the referral discount to your account — the program advertises 5% off for referred users.

👉 Unlock the referral discount on your 9Proxy account

## Two models, and the difference is bigger than it looks

|  | Residential by IPs | Residential by GB |
| --- | --- | --- |
| Billing | Per IP, fixed package | Per GB of traffic |
| Traffic | Unlimited while the IP is active | Limited by purchased GB |
| Validity | Unused IPs never expire | 180 days, unlimited on Enterprise tiers |
| IP behaviour | No natural rotation; rotates via auto-rotation ports | Rotating or sticky via username parameters |
| Authentication | 9Proxy desktop app (local port forwarding) | Username/password or IP whitelist |
| Setup | Desktop app required | Straight from the dashboard |

A detail worth reading twice: on the IP-based model, each individual IP stays alive for a few hours up to about 24 hours, depending on the address. That's normal for residential IPs, and the workaround is built in — unused IPs don't expire, so you buy a pool and draw from it over time. A forum thread on the brand's own reseller channel shows a user complaining about slow speeds, with support replying that throughput depends on your local connection and the target site. Take that as a fair warning that residential IP speed in Korea is variable, not as a dealbreaker.

## Every 9Proxy package, side by side

Usage is balance-based, so packages stack onto one account rather than replacing each other.

| Model | Package | Traffic / validity | Price | Get it |
| --- | --- | --- | --- | --- |
| IP-based | 100 IPs | Unlimited bandwidth per IP | $24 ($0.24/IP) | Start with 100 IPs |
| IP-based | 500 IPs | Unlimited bandwidth per IP | $72 ($0.144/IP) | Buy the 500 IP pack |
| IP-based | 1,000 + 500 bonus IPs | Unlimited bandwidth per IP | $126 ($0.084/IP) | Grab the 1,500 IP bundle |
| IP-based | 2,500 IPs | Unlimited bandwidth per IP | $210 ($0.084/IP) | Get 2,500 IPs |
| IP-based | 5,000 IPs | Unlimited bandwidth per IP | $360 ($0.072/IP) | Buy 5,000 IPs |
| IP-based | 15,000 IPs | Unlimited bandwidth per IP | $720 ($0.048/IP) | Scale to 15,000 IPs |
| IP-based | 25,000 IPs | Unlimited bandwidth per IP | $863 ($0.035/IP) | Choose the 25,000 IP tier |
| IP-based | 50,000 IPs | Unlimited bandwidth per IP | $1,438 ($0.029/IP) | Check the 50,000 IP package |
| Business IP | 100,000 IPs | Unlimited bandwidth per IP | $2,300 ($0.023/IP) | See the 100,000 IP volume tier |
| Business IP | 200,000 IPs | Unlimited bandwidth per IP | $4,140 ($0.021/IP) | Compare the 200,000 IP tier |
| Business IP | 500,000 IPs | Unlimited bandwidth per IP | $8,625 ($0.018/IP) | Request the 500,000 IP tier |
| GB-based | 5 GB | 5 GB, 180 days | $15 ($3.00/GB) | Buy 5 GB to test |
| GB-based | 50 + 5 bonus GB | 55 GB, 180 days | $105 ($2.10/GB) | Get the 55 GB pack |
| GB-based | 100 GB | 100 GB, 180 days | $150 ($1.50/GB) | Pick the 100 GB plan |
| GB-based | 200 GB | 200 GB, 180 days | $200 ($1.00/GB) | Buy 200 GB |
| GB-based | 1,000 GB | 1,000 GB, 180 days | $800 ($0.80/GB) | Go for 1,000 GB |
| GB-based | 2,000 GB | 2,000 GB, 180 days | $1,500 ($0.75/GB) | Order 2,000 GB |
| Enterprise GB | 3,000 GB | Never expires | $2,160 ($0.72/GB) | Review the 3,000 GB tier |
| Enterprise GB | 6,000 GB | Never expires | $4,200 ($0.70/GB) | See the 6,000 GB tier |
| Enterprise GB | 10,000 GB | Never expires | $6,800 ($0.68/GB) | Check the 10,000 GB tier |
| Bundle | Starter — 100 IPs + 5 GB | 180 days on traffic | $30 | Buy the Starter bundle |
| Bundle | Popular — 1,500 IPs + 50 GB | 180 days on traffic | $180 | Buy the Popular bundle |
| Bundle | Pro — 5,000 IPs + 500 GB | 180 days on traffic | $720 (list $860) | Buy the Pro bundle |

Two notes on how to read that: the IP-based and bundle prices above reflect the adjustment the company announced for June 1, 2026, while GB-based pricing stayed where it was. And the smallest per-IP package is 100 IPs — there's no five-IP starter, which matters if you only need two or three Korean addresses.

## How you actually route traffic through a Korean IP

The two models are set up differently, which is the single most common source of confusion.

With **Residential by GB**, all targeting lives in the username. There's no app to install. The format is:


<sub-user>-country-<code>-st-<state>-city-<name>-isp-<code>-sst-<minutes>-ssid-<id>


A rotating Korean exit, one fresh IP per request:


youruser-country-kr


A sticky Korean exit held for 20 minutes, which is what you'd want for a logged-in Korean session:


youruser-country-kr-sst-20


And in code, it's one line change:

python
proxy = "http://youruser-country-kr-sst-20:yourpassword@your_proxy_host:your_port"


Over-filtering is the trap. Adding city and ISP on top of country shrinks the Korean address pool and can return slower or failed requests. Start at country level and tighten only when your data actually needs it.

With **Residential by IPs**, you install the 9Proxy app, filter the available list by Country, State, City, ZIP code or ISP, then forward the address you want to a local port. Press `F` to filter, select a proxy, hit Enter and forward it to a single port or your whole configured range. From the command line:


9proxy proxy -c KR -p 60000


That binds a Korean residential IP to `127.0.0.1:60000` and it's live immediately. Test it before you build anything on top:


curl -x socks5://127.0.0.1:60000 https://ipinfo.io/json


If the result shows a Korean location, you're working. One genuinely useful feature here: the Today List, which holds every IP you've used in the last 24 hours (`9proxy proxy -n -p 60000`). Reusing an address from that list doesn't consume a new one, so a Korea project that runs daily can cycle through a smaller pool than you'd expect.

Want to see how the filtering looks against your own targets first?

👉 Set up a 9Proxy account and test Korean exits yourself

## What Korean work actually looks like

These are the tasks where Korean IPs are the barrier, not a nice-to-have.

**Naver rank tracking.** Naver's results differ from Google's, and they change by location inside Korea. Country-level targeting gets you the national picture; anything more local needs city or ZIP filtering.

**Naver Blog, Cafe and Shopping access.** These services restrict what non-Korean visitors see. If your competitive research depends on what a Korean user sees in Naver Shopping, you need a Korean exit to see it.

**Coupang price and stock monitoring.** Domestic pricing and delivery estimates, guarded by rate limiting. Rotating Korean residential IPs spread across many sessions handle this better than a handful of static addresses.

**Korean ad verification.** Campaign previews often fail to render, or render as fallback creative, when the requesting IP is in the wrong country. Verifying Korean placements requires Korean exits, and the proof is a rendered ad, not a screenshot from your desk.

**Game and release-window access.** Korean gaming platforms and sneaker drops are country-gated and reputation-sensitive. Clean residential or mobile Korean addresses are the only thing that reliably passes.

**Localisation QA.** Checking KRW pricing, regional delivery options and translated copy as an actual Korean visitor sees them.

If any of that involves signed-in accounts, check the platform's terms first — it's the account policy that constrains you, not the proxy.

## Where it doesn't fit

Be honest with yourself about three things before buying.

The IP-based model requires the desktop app for local port forwarding. There's no way to pop a Korean IP straight out of the dashboard on that model, which rules out some headless server setups.

Korean IP availability inside a shared global pool is less predictable than from a vendor that sells Korea as a dedicated product with carrier ASN targeting. If your project needs a specific Korean ISP, verify that filtering matches your target before committing to a large package — a 5 GB pack at $15 costs far less than discovering the mismatch after a 1 TB purchase.

And speed follows the address, not the brand. Residential IPs are real consumer connections, so throughput varies. A third-party review of the network reported roughly 0.6-second average response times and around a 99.5% success rate in its own testing, but your results depend on the specific Korean IP you draw and the site you're hitting.

## Picking a package for Korean work

For a first run, 5 GB at $15 is the sensible entry point. It's enough to confirm that Korean exits resolve, that your parser reads Naver or Coupang correctly, and that your success rate is acceptable — before spending anything meaningful. Traffic is valid for 180 days, so a slow start costs you nothing but time.

If you've confirmed the approach and you're scraping daily, 100 GB at $150 or 200 GB at $200 covers most single-target monitoring setups for months.

If your Korean work is session-based — logged into accounts, browsing heavy pages, long-running automation — the per-IP model is the better economics: 100 IPs for $24 with no bandwidth ceiling, or 500 IPs for $72 if you're running parallel profiles. Each address lives a few hours to a day, and unused ones don't expire, so the pool drains at your pace.

Mixed workloads where some jobs need stable sessions and others need volume are what the bundles are for. The $30 Starter pack pairs 100 IPs with 5 GB and is a reasonable way to decide which half of the account you actually use.

One more thing worth knowing: no monthly commitment, no auto-renewing subscription, and payment options include cards, crypto, bank transfer, Alipay, Apple Pay and Google Pay. Support runs 24/7 per the company, and trial access for new users is offered in limited quantities depending on availability — worth asking about if you'd rather test before paying.

Ready to check whether Korean exits show up in the locations you need?

👉 Create your 9Proxy account and get the referral discount
