# ⛏ Bitcoin Miner Hosting ROI Comparison

A live, interactive comparison tool for Bitcoin ASIC mining hosting companies. Compare rates, ROI projections, host margins, community reviews, pool freedom, and brand compatibility across all major hosts — with a live BTC price feed.

**[→ Open the Live Tool](https://blackshirt-crypto.github.io/miner-hosting-comparison/)**

---

## What it does

- **Live BTC price** via CoinGecko / Binance / CoinCap fallback chain
- **ROI calculator** — daily net profit, monthly, annual, and 3-year projections
- **Sats mined per day** alongside USD value at current price
- **Host margin / repair buffer** — estimates what hosts pay vs what you pay
- **Community Signal** — independent third-party reviews (Trustpilot, Reddit, forums) with click-to-expand details
- **Stratum / Pool Freedom** — can you point your miner at BCH, solo, or any SHA-256 endpoint?
- **Brand compatibility** — which ASIC brands each host accepts
- **Add & edit hosts** — add new companies you discover with full rate modeling
- **BTC difficulty growth slider** — model what happens to your ROI if network hashrate increases

---

## Data

All host data lives in [`blackshirt-crypto.json`](./blackshirt-crypto.json). The **Last Updated** date in the tool header reflects the last time this file was pushed to the repo.

Community contributions live in [`community-notes.json`](./community-notes.json). See [CONTRIBUTING.md](./CONTRIBUTING.md) for how to submit a note.

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
| Sazmining | Paraguay/Ethiopia | ~$0.060/kWh | ⚠️ Luxor/OCEAN only |
| ASL Miner | Russia | $0.065/kWh | ❓ Unconfirmed |

---

## Updating the Data

If you maintain this tool, see the update workflow:

1. Run a research session (check host websites, Trustpilot, Reddit)
2. Edit `blackshirt-crypto.json` with updated rates, notes, signals
3. Push to GitHub — the live tool updates automatically
4. Review any pending Pull Requests to `community-notes.json`

---

## Disclaimer

Data is researched manually and reflects conditions at the **Last Updated** date shown in the tool. BTC price is live. Host rates, terms, and availability change — always verify directly with the host before committing capital. This is not financial advice.

---

*Maintained by blackshirt-crypto*
