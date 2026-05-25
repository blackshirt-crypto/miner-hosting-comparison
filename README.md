# ⛏ Bitcoin Miner Hosting ROI Comparison

A live, interactive comparison tool for Bitcoin ASIC mining hosting companies. Compare rates, ROI projections, host margins, community reviews, pool/stratum freedom, and brand compatibility — with a live BTC price feed.

**[→ Open the Live Tool](https://blackshirt-crypto.github.io/miner-hosting-comparison/)**

---

## What it does

- **Live BTC price** via CoinGecko / Binance / CoinCap fallback chain — auto-refreshes every 60 seconds
- **ROI calculator** — daily net profit, monthly, annual, and 3-year projections with difficulty growth modeling
- **Sats mined per day** alongside USD value at current BTC price
- **Host margin / repair buffer** — estimates what hosts pay for power vs what you pay them
- **Community Signal** — independent third-party reviews (Trustpilot, Reddit, forums) with click-to-expand details. Not company testimonials.
- **Pool / Stratum Freedom** — can you point your miner at any SHA-256 stratum endpoint? BCH pools, solo mining, custom endpoints? Click to expand per host.
- **Brand compatibility** — which ASIC brands (Bitmain, MicroBT, Canaan, etc.) each host accepts
- **Add & Edit hosts** — add new companies you find with full rate modeling; edit any existing host when rates change
- **Difficulty growth slider** — model what happens to your ROI as network hashrate increases over 3 years
- **📅 Last Updated badge** — shows when the host data was last researched and pushed

---

## Data files

| File | Purpose | Who edits |
|------|---------|-----------|
| `blackshirt-crypto.json` | Master host data — rates, notes, signals, pool policy | blackshirt-crypto only |
| `community-notes.json` | Community-contributed customer experiences | Open via Pull Request |

The **Last Updated** date in the tool header reflects the last push to `blackshirt-crypto.json`. BTC price is always live.

---

## Current Hosts Tracked

| Host | Location | Rate | Pool Freedom |
|------|----------|------|-------------|
| Simple Mining | Iowa, USA | $0.075/kWh | ✅ Any |
| Compass Mining | 22 farms, USA | $0.085/kWh | ✅ Any |
| Bitkern | USA + global | $0.0795/kWh | ❓ Unconfirmed |
| Lonestar Miners | Texas, USA | $0.09/kWh | ❓ Unconfirmed |
| Terra Hosting | Indiana, USA | $0.0825/kWh | ✅ Any |
| BT-Miners | USA | $0.105/kWh | ❓ Unconfirmed |
| Abundant Mines | Oregon, USA | Contact | ✅ Any |
| AsicHive | USA | Contact | ❓ Unconfirmed |
| Block Ops Mining | Arkansas, USA | Contact | ❓ Unconfirmed |
| DataPrana | Iowa + Texas, USA | Contact | ❓ Unconfirmed |
| Sazmining | Paraguay/Ethiopia/S.Dakota | ~$0.060/kWh | ⚠️ Luxor/OCEAN only |
| ASL Miner | Russia | $0.065/kWh + op fee | ❓ Unconfirmed |

---

## Updating the data

When rates, terms, or review data changes:

1. Edit `blackshirt-crypto.json` — update the relevant host's `rate`, `notes`, `poolDetails`, or signal data
2. Update `meta.last_updated` to today's date
3. `git add blackshirt-crypto.json && git commit -m "Rate/data update YYYY-MM-DD" && git push`
4. The live tool updates automatically within seconds — no HTML changes needed

For feature additions (new columns, UI changes): update `index.html` and push alongside the JSON.

---

## Contributing community notes

See [CONTRIBUTING.md](./CONTRIBUTING.md) for how to submit a real customer experience, rate confirmation, or correction via Pull Request to `community-notes.json`.

---

## Disclaimer

Data is researched manually and reflects conditions at the **Last Updated** date shown in the tool. BTC price is live via public APIs. Host rates, terms, and availability change — always verify directly with the host before committing capital. This is not financial advice.

---

*Maintained by [blackshirt-crypto](https://github.com/blackshirt-crypto)*
