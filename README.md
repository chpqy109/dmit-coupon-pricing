# vps coupon: How to Spot Recurring DMIT Codes That Still Work, Which Plans They Cover, and the Full LAX/HKG/TYO Price Table

Most "vps coupon" pages are useless in a very specific way. You get a wall of codes with no indication of which product line, which billing term, or which year they were issued for, and you find out they're dead at the last step of checkout, after you've already picked a plan and typed your card number.

That's the problem worth solving. So this is less a coupon dump and more a working method: what kind of discounts actually exist at DMIT, how to tell a live code from a dead one before you commit, and what every currently listed plan costs so you know whether the discount is even worth chasing.

DMIT (dmit.io) is the provider here. US-registered, Chinese-speaking team, VPS in Los Angeles, Hong Kong and Tokyo, and a reputation for network routes rather than cheap hardware. It is also, notably, not a shop that runs permanent "50% off everything" banners. Its promo rhythm is closer to occasional, targeted, and term-limited.

## Why the coupon list you found probably doesn't work

A quick note on mechanics, because it explains most of the frustration.

DMIT runs its billing on WHMCS, the same platform behind a large chunk of the hosting industry. That means two separate things can reduce your price at checkout:

- **Billing-cycle discounts**, which are built into the product and applied automatically when you pick a longer term. No code required. On several DMIT lines, annual billing alone knocks a meaningful percentage off, and the LAX Pro entry plan has had a deeper automatic annual discount than the rest of the family.
- **Promotional codes**, which you paste into the checkout field and validate manually. These are the ones that expire, and they're the ones every "vps coupon" list is really talking about.

The codes worth caring about are the ones ending in `RECURRING`. Those apply to renewals, not just the first invoice, which is the difference between saving money once and saving money every year you keep the server. If you're comparing two codes and only one recurs, the recurring one usually wins even at a smaller percentage.

The other thing to know: DMIT scopes its codes tightly. A code issued for Tokyo Tier 1 will not touch a Hong Kong Premium plan. Copy-pasting a code from a generic coupon aggregator onto the wrong product is the single most common reason people think a code "doesn't work."

## Coupon codes reported by community trackers

The codes below are the ones that appear consistently across multiple independent VPS deal trackers. Treat this as a starting shortlist to validate, not as a guarantee — community-maintained lists lag behind actual expiry, and DMIT's own promo windows have historically been narrow.

| Code | Applies to | Billing term | Discount |
| --- | --- | --- | --- |
| `LAX-EB-LAUNCH-NON-MONTHLY-RECURRING-20OFF` | Los Angeles Eyeball, TINY and up | Quarterly or longer | 20% recurring |
| `202510_HKG_TYO_PRO_20OFF_RECURRING` | Hong Kong / Tokyo Premium (Pro) | Quarterly or longer | 20% recurring |
| `202510_HKG_TYO_T1_30OFF_RECURRING` | Hong Kong / Tokyo Tier 1, excluding WEE | Quarterly or longer | 30% recurring |
| `2025-TYO-T1-HI-GSL-NON-MONTHLY-30OFF` | Tokyo Tier 1, TINY and up | Quarterly or longer | 30% |
| `2025-TYO-T1-HI-GSL-MONTHLY-10OFF` | Tokyo Tier 1, TINY and up | Monthly | 10% |
| `2025-XMAS-LAX-PRO-EB-ANNUALLY-STARTER-AND-HIGHER-15OFF-RECURRING` | LAX Pro / Eyeball, STARTER and up | Annual | 15% recurring, plus credit back |
| `2025-XMAS-LAX-PRO-EB-10-OFF-RECURRING` | LAX Pro / Eyeball | Any regular term | 10% recurring, plus credit back |
| `2025-XMAS-LAX-T1-10-OFF-RECURRING` | LAX Tier 1, excluding WEE | Any regular term | 10% recurring, plus credit back |
| `Lite-Annually-Recur-30OFF` | Standard/Lite network lines | Annual | 30% recurring |
| `Lite-Semi-Annually-Recur-20OFF` | Standard/Lite network lines | Semi-annual | 20% recurring |

If you want to test one against live stock and pricing rather than reading about it, 👉 [👉 open DMIT's current plan list and test a code at checkout](https://www.dmit.io/aff.php?aff=12046).

## How to check a code is live before you pay

Four steps, in order. Skipping to step four is what wastes money.

1. Pick the plan and the billing term first. The term changes which codes are eligible, so choosing monthly and then hunting for a code gets you nowhere.
2. Paste the code into the checkout field exactly as written and hit validate. The system will accept it, reject it, or apply a different discount than you expected.
3. Read the discount line, not just the "valid" confirmation. A code can be accepted and still be worth less than the automatic billing-cycle discount already applied.
4. Confirm the renewal price. If the code doesn't carry the `RECURRING` tag, you're looking at a first-invoice discount and the full price next term.

One more thing worth checking: DMIT has run "credit back" promos where a percentage of your payment returns to your account balance in monthly instalments over twelve months. That's not the same as a discount. It's store credit you can spend later. If a code advertises a combined figure like "15% off plus 10% cashback," the effective saving only materialises if you actually use the balance.

## The full plan and price rundown

This is where most coupon articles stop being useful, because DMIT's catalogue is genuinely confusing: three regions, three network families per region, and two or three hardware platform generations layered on top. The same nominal plan can differ by 15–30% in price depending on whether it sits on the older EPYC 7003 (AS3), EPYC 9004 (AN4), or EPYC 9005 (AN5) platform.

The three network families, in plain terms:

- **Premium (Pro)** — routes built around China Telecom's CN2 GIA, with transit and backbone resources layered in. The premium tier, aimed at traffic to and from mainland China and Asia-Pacific.
- **Eyeball (EB)** — CMIN2 and AS9929 based. Cheaper than Pro, and typically more generous on traffic for the same money.
- **Tier 1 (T1)** — international BGP with no mainland China optimisation at all. Cheapest, biggest ports, biggest traffic allowances.

Prices below reflect the figures most consistently reported across trackers, with ranges shown where sources disagree on the current platform pricing. Stock on this provider moves fast — individual plans sell out and reappear regularly — so treat the table as a map and the checkout page as the territory.

### Los Angeles (LAX)

AMD EPYC platforms, KVM virtualisation, 1 IPv4 plus a /64 IPv6 block on the standard plans.

| Plan | vCPU / RAM / SSD | Traffic & port | Overage behaviour | Price | Check stock |
| --- | --- | --- | --- | --- | --- |
| LAX.T1.WEE | 1 / 1GB / 20GB | 1TB @ 4Gbps | 100Mbps unmetered | $36.90/year | [ See LAX Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| LAX.T1.TINY | 1 / 1GB / 20GB | 2TB @ 4Gbps | 200Mbps unmetered | $6.90/month | [ See LAX Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| LAX.T1.STARTER | 1–2 / 2GB / 40GB | 4TB @ 10Gbps | 200Mbps unmetered | $12.90/month | [ See LAX Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| LAX.T1.MINI | 2 / 2GB / 60GB | 8TB @ 10Gbps | 200Mbps unmetered | $21.90/month | [ See LAX Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| LAX.T1.MICRO | 4 / 4GB / 80GB | 16TB @ 10Gbps | 500Mbps unmetered | $32.90/month | [ See LAX Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| LAX.T1.MEDIUM | 4 / 8GB / 160GB | 32TB @ 10Gbps | 500Mbps unmetered | $49.90/month | [ See LAX Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| LAX.T1.LARGE | 8 / 16GB / 320GB | 64TB @ 10Gbps | 500Mbps unmetered | $99.90/month | [ See LAX Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| LAX.T1.GIANT | 8 / 24GB / 640GB | 128TB @ 10Gbps | 1Gbps unmetered | $199.90/month | [ See LAX Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| LAX.Pro.TINY | 1 / 2GB / 20GB | 1TB @ 1Gbps | 4Mbps unmetered | $10.90/mo (AS3) – $12.98/mo (AN5) | [ See LAX Premium](https://www.dmit.io/aff.php?aff=12046) |
| LAX.Pro.Pocket | 2 / 2GB / 40GB | 1.5TB @ 4Gbps | 4Mbps unmetered | $16.90/month | [ See LAX Premium](https://www.dmit.io/aff.php?aff=12046) |
| LAX.Pro.STARTER | 2 / 2GB / 80GB | 3TB @ 10Gbps | 4Mbps unmetered | $34.90/month | [ See LAX Premium](https://www.dmit.io/aff.php?aff=12046) |
| LAX.Pro.MINI | 4 / 4GB / 80GB | 5TB @ 10Gbps | 8Mbps unmetered | $62.90/month | [ See LAX Premium](https://www.dmit.io/aff.php?aff=12046) |
| LAX.Pro.MICRO | 4 / 4GB / 160GB | 7TB @ 10Gbps | 8Mbps unmetered | $87.90/month | [ See LAX Premium](https://www.dmit.io/aff.php?aff=12046) |
| LAX.Pro.MEDIUM | 6 / 8GB / 160GB | 14TB @ 10Gbps | 10Mbps unmetered | $199.90/month | [ See LAX Premium](https://www.dmit.io/aff.php?aff=12046) |
| LAX.EB.TINY | 1 / 2GB / 20GB | 1.5TB @ 2Gbps | 4Mbps unmetered | $10.90/month | [ See LAX Eyeball](https://www.dmit.io/aff.php?aff=12046) |
| LAX.EB.Pocket | 2 / 2GB / 40GB | 3TB @ 4Gbps | 4Mbps unmetered | $16.90/month | [ See LAX Eyeball](https://www.dmit.io/aff.php?aff=12046) |
| LAX.EB.STARTER | 2 / 2GB / 80GB | 5TB @ 10Gbps | 4Mbps unmetered | $34.90/month | [ See LAX Eyeball](https://www.dmit.io/aff.php?aff=12046) |

### Hong Kong (HKG)

Physically closest to mainland China, and priced accordingly on the Pro line.

| Plan | vCPU / RAM / SSD | Traffic & port | Overage behaviour | Price | Check stock |
| --- | --- | --- | --- | --- | --- |
| HKG.T1.WEE | 1 / 1GB / 20GB | 1TB @ 4Gbps | 50Mbps unmetered | $36.90/year | [ See HKG Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.TINY | 1 / 1GB / 20GB | 2TB @ 4Gbps | 100Mbps unmetered | $6.90/month | [ See HKG Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.STARTER | 1 / 2GB / 40GB | 4TB @ 10Gbps | 100Mbps unmetered | $12.90/month | [ See HKG Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.MINI | 2 / 2GB / 60GB | 8TB @ 10Gbps | 100Mbps unmetered | $21.90/month | [ See HKG Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.MICRO | 4 / 4GB / 80GB | 16TB @ 10Gbps | 200Mbps unmetered | $32.90/month | [ See HKG Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.MEDIUM | 4 / 8GB / 160GB | 32TB @ 10Gbps | 200Mbps unmetered | $49.90/month | [ See HKG Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.LARGE | 8 / 16GB / 320GB | 64TB @ 10Gbps | 500Mbps unmetered | $99.90/month | [ See HKG Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| HKG.T1.GIANT | 8 / 24GB / 640GB | 128TB @ 10Gbps | 1Gbps unmetered | $199.90/month | [ See HKG Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.TINY | 1 / 1GB / 20GB | 500GB @ 1Gbps | Suspended on overage | $39.90/month | [ See HKG Premium](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.STARTER | 1 / 2GB / 40GB | 1TB @ 1Gbps | Suspended on overage | $79.90/month | [ See HKG Premium](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.MINI | 2 / 2GB / 60–80GB | 1.5TB @ 1Gbps | Suspended on overage | $119.90–149.90/month | [ See HKG Premium](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.MICRO | 2 / 4GB / 80–160GB | 2TB @ 1Gbps | Suspended on overage | $159.90–179.90/month | [ See HKG Premium](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.MEDIUM | 4 / 4GB / 160GB | 2.5TB @ 1Gbps | Suspended on overage | $180–239.90/month | [ See HKG Premium](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.LARGE (AN5) | 4 / 8GB / 320GB | 3TB @ 1Gbps | Suspended on overage | $240/month | [ See HKG Premium](https://www.dmit.io/aff.php?aff=12046) |
| HKG.Pro.GIANT (AN5) | 8 / 16GB / 640GB | 6TB @ 1Gbps | Suspended on overage | $500/month | [ See HKG Premium](https://www.dmit.io/aff.php?aff=12046) |

The wide ranges on HKG Pro are not sloppiness. Sources tracking the AS3 and AN5 platforms report different figures for the same slot, and the platform mix on the shelf changes month to month. Check the live page before you build a budget around any single number.

### Tokyo (TYO)

Note that the Tokyo Eyeball line has been retired. Tokyo now runs Premium and Tier 1.

| Plan | vCPU / RAM / SSD | Traffic & port | Overage behaviour | Price | Check stock |
| --- | --- | --- | --- | --- | --- |
| TYO.T1.WEE | 1 / 1GB / 20GB | 1TB @ 4Gbps | 50Mbps unmetered | $36.90/year | [ See TYO Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.TINY | 1 / 1GB / 20GB | 2TB @ 4Gbps | 100Mbps unmetered | $6.90/month | [ See TYO Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.STARTER | 1 / 2GB / 40GB | 4TB @ 10Gbps | 100Mbps unmetered | $12.90/month | [ See TYO Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.MINI | 2 / 2GB / 60GB | 8TB @ 10Gbps | 100Mbps unmetered | $21.90/month | [ See TYO Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.MICRO | 4 / 4GB / 80GB | 16TB @ 10Gbps | 200Mbps unmetered | $32.90/month | [ See TYO Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.MEDIUM | 4 / 8GB / 160GB | 32TB @ 10Gbps | 200Mbps unmetered | $49.90/month | [ See TYO Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.LARGE | 8 / 16GB / 320GB | 64TB @ 10Gbps | 500Mbps unmetered | $99.90/month | [ See TYO Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.GIANT | 8 / 24GB / 640GB | 128TB @ 10Gbps | 1Gbps unmetered | $199.90/month | [ See TYO Tier 1](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.TINY | 1 / 1GB / 20GB | 500GB @ 1Gbps | Suspended on overage | $21.90/month | [ See TYO Premium](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.STARTER | 1 / 2GB / 40GB | 1TB @ 1Gbps | Suspended on overage | $39.90–45.90/month | [ See TYO Premium](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.MINI | 2 / 4GB / 60GB | 2TB @ 1Gbps | Suspended on overage | $89.90/month | [ See TYO Premium](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.MICRO | 4 / 4GB / 80GB | 4TB @ 1Gbps | Suspended on overage | $189.90/month | [ See TYO Premium](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.MEDIUM | 4 / 8GB / 160GB | 6TB @ 1Gbps | Suspended on overage | $320.90/month | [ See TYO Premium](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.LARGE | 8 / 16GB / 320GB | 8TB @ 1Gbps | Suspended on overage | $429.90/month | [ See TYO Premium](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.GIANT | 8 / 24GB / 640GB | 15TB @ 1Gbps | Suspended on overage | $829.90/month | [ See TYO Premium](https://www.dmit.io/aff.php?aff=12046) |

One detail that matters more than the price table: the Premium line suspends your service when you exceed the traffic allowance, while Tier 1 and Eyeball plans drop you to a throttled speed and keep running. If you're running something that can't go offline, that difference is worth more than a 10% coupon.

## Where a coupon actually changes the math

Take LAX Eyeball TINY at $10.90/month. A 20% recurring discount applied to a quarterly term brings the quarterly invoice from $32.70 to $26.16, and that reduction repeats. Over a year on quarterly billing, the gap is roughly $26. If you'd otherwise have bought monthly, the code plus the term change together do more work than the code alone.

Now take HKG Tier 1 WEE at $36.90/year. It's already the cheapest annual entry in the catalogue, and at that price point a 10% coupon saves about $3.70 a year. Hunting for a code there isn't a bad idea, but it shouldn't be the reason you choose that plan over something better suited to your traffic pattern. The plan choice is worth hundreds of dollars a year. The coupon is worth tens.

That's the honest hierarchy: get the network family and the region right first, then optimise with codes.

## Before you check out

A few terms worth knowing, since they affect whether a discounted purchase is a good deal.

- **Refunds.** Reports describe a full refund window of three days if total traffic use stays under 30GB, and pro-rated refunds within 30 days. Renewal orders and payments made from account balance have been reported as non-refundable. Three days is short. Test the route during that window, not after.
- **IP replacement.** If your assigned IP stops working for your use case, Pro and Eyeball plans have been reported as allowing a free swap once every 15 days, with additional swaps charged at $5. Cheaper than re-provisioning the server.
- **Stock volatility.** DMIT deliberately limits how many instances it sells per hardware batch, which is why plans go out of stock in hours and reappear weeks later. A plan listed as available while you read this may not be available while you decide.
- **Payment methods.** Alipay, WeChat Pay, PayPal, credit cards and, per several trackers, crypto. The Alipay support is why the provider has such a large Chinese-speaking user base.
- **Platform caveat.** LAX AS3 hardware has carried an official note that the platform is still under optimisation, with possible disk performance and SLA differences compared to mature platforms. If you're deploying something that can't tolerate that, test first.

## Questions that come up repeatedly

**Does DMIT ever run a sitewide discount?**
Not in the way budget hosts do. Its promotions are usually scoped to a product line, a region, or a billing term, and the automatic annual discounts on some lines are larger than any code you'll find.

**Is it worth paying annually to get the discount?**
Only after you've tested. Annual saves the most and locks the rate, but a 3-day refund window means a year of regret if the route doesn't suit your ISP. Buy monthly first, confirm the route works, then decide.

**Which line should a mainland-China-facing project buy?**
Premium. It's the line built around CN2 GIA. Eyeball is the compromise tier, and Tier 1 has no China optimisation at all, which surprises people who assume "Hong Kong" implies low mainland latency. It doesn't.

**Do the codes stack?**
No. Checkout takes one code. If two codes look attractive, validate both and keep whichever produces the lower renewal price.

If you'd rather run the numbers yourself, 👉 [👉 check live DMIT pricing and validate a coupon on the plan you actually want](https://www.dmit.io/aff.php?aff=12046) — the checkout page is the only place where the discount, the term and the stock status are all simultaneously true.
