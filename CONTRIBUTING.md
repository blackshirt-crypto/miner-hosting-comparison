# Contributing to Bitcoin Miner Hosting ROI Comparison

Thanks for helping keep this data accurate. Here's how it works.

---

## Two files, two purposes

**`blackshirt-crypto.json`** — the authoritative master data. Maintained by blackshirt-crypto. Branch-protected. You cannot push to it directly.

**`community-notes.json`** — open for community contributions via Pull Request. This is where you add your real customer experiences, rate corrections, and observations.

---

## How to submit a community note

1. **Fork** this repository
2. Open `community-notes.json`
3. Add your entry to the `notes` array following the schema below
4. Submit a **Pull Request** with a clear title like `[Terra Hosting] Rate still $0.0825 as of May 2026`

---

## Schema

```json
{
  "host": "Exact company name as shown in the tool",
  "contributor": "your_github_username",
  "date": "2026-05-24",
  "type": "rate_update",
  "note": "Your specific, factual observation.",
  "verified": false,
  "source": "https://optional-url-if-you-have-one.com"
}
```

### Type options

| Type | Use for |
|------|---------|
| `rate_update` | Confirming or correcting a $/kWh or monthly rate |
| `customer_experience` | Personal hosting experience — uptime, support, repairs |
| `pool_policy` | Confirming which pools/stratum endpoints are allowed |
| `brand_policy` | Confirming which ASIC brands a host accepts |
| `warning` | A negative experience or structural risk others should know |
| `correction` | Factual error in the current data |

---

## What makes a good submission

✅ **Specific and dated** — "Confirmed $0.0825/kWh as of May 2026 via email with Mike"  
✅ **Real customer experience** — "My S21 XP has been hashing at Terra since January, 98% uptime"  
✅ **Pool/brand confirmation** — "Confirmed with support that they accept WhatsMiner M66 units"  
✅ **Factual corrections** — "Rate changed to $0.08/kWh in April 2026 per their updated pricing page"  

❌ **Marketing copy** — anything that reads like a company pitch  
❌ **Unverifiable claims** — "I heard they had problems" without specifics  
❌ **Company employees submitting positive reviews** — obvious self-promotion gets rejected  
❌ **Speculative** — opinions about future profitability or market conditions  

---

## Review process

The maintainer (blackshirt-crypto) reviews Pull Requests periodically — typically monthly or after a research update session. Accepted notes may be:

- Displayed as "community verified" in the live tool
- Promoted into `blackshirt-crypto.json` if they represent a confirmed data update

Notes that cannot be verified or appear promotional will be politely declined with an explanation.

---

## What you cannot change

`blackshirt-crypto.json` is branch-protected. Any PR touching that file will be rejected. If you believe there is a factual error in the master data, submit a `correction` type note in `community-notes.json` explaining the discrepancy — the maintainer will verify and update.

---

*Questions? Open an Issue.*
