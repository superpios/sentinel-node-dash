# Sentinel Node Dash

An arcade endless-runner that teaches the Sentinel dVPN ecosystem while you play — powered by live node data.

**▶ Play: https://superpios.github.io/sentinel-node-dash/**

## What it is

You are a data packet running through the Sentinel decentralized bandwidth network.

- ⚡ **Collect real nodes.** Every node orb is a live Sentinel node pulled from the [Node Scorecard](https://superpios.github.io/node-scorecard/) — real moniker, real country, real download speed, real protocol (WireGuard and V2Ray today, plus the first Xray, Hysteria2 and AmneziaWG pioneer nodes), and an official **SLA ✓** badge when a node has passed the network's real-world speed test.
- ⭐ **Score multipliers reflect real-world privacy.** Collecting a residential node (a real home IP) gives a **2.4×** score bonus because residential IPs are the top privacy tier — they look like an ordinary user, so they're far harder to block. Datacenter nodes give a **1.2×** bonus for their speed, despite known IP ranges.
- ⚠️ **Dodge the censorship bricks.** DPI, trackers, ISP logs, geo-blocks, throttling.
- 🧠 **Learn while you play — 31 topics.** A short tutorial shows the controls at the start of every run. Every few stars a new topic is revealed, followed by a quiz. Answer correctly and you earn bonus $P2P and score — or, on technical topics (protocols, privacy, security, node types, AI-agent payments), a temporary **power-up**: ⛨ **WireGuard Mode** (5 seconds of invincibility) or ⚡ **P2P Boost** (12 seconds of double score).

Topics cover the dVPN apps built on Sentinel (Sentinel Shield, Independent VPN, Ryn VPN, DVPN by NORSE, VALT, Meile, ChibaTunnel), the tools and explorers (BlueCLI, P2PScan, SuchNode, Network Stats, Node Scorecard), the community (Bluefrens), core concepts (on-chain sessions, $P2P, WireGuard/V2Ray, the new anti-censorship protocol wave, official SLA tests, x402 payments for AI agents), and deep dives into privacy, security by design, and how to build your own VPN brand on open infrastructure.

Each topic — and its quiz — appears only once per run. Once you've seen them all, stars become pure bonus and the game stops interrupting you.

> **Note on in-game currency:** any mention of $P2P within the game (multipliers, values) is purely educational and represents virtual points — no real cryptocurrency is earned, paid out, or expected.

## Controls

| Action | Keys |
|---|---|
| Jump (double jump!) | `Space` · `↑` · `W` · tap / click |
| Pause | `P` · `Esc` |
| Restart run | `R` (while paused or on game over) |
| Main menu | `M` (while paused or on game over) |
| Start | `Enter` |

Three player skins to choose from: **Data Packet**, **dVPN Shield**, **$P2P Coin**.

## Tech

- **Single HTML file.** No build step, no framework, no CDN, no dependencies.
- **One outbound request, ever:** the public Node Scorecard JSON. Nothing else leaves your browser.
- **No tracking, no analytics, no cookies, no accounts.** The only thing stored is your high score, kept in `localStorage` on your own device — it is never sent anywhere, and clearing your site data wipes it.
- **Audio is synthesized in-browser** with the Web Audio API — no media files.
- **All artwork is original vector art** drawn on `<canvas>`. No third-party logo or trademark file is embedded.
- **Falls back to demo node data** if the Scorecard is unreachable, so the game always runs. The menu tells you which mode you're in (● LIVE or ○ Offline).

## Run locally

```bash
git clone https://github.com/superpios/sentinel-node-dash.git
cd sentinel-node-dash
python3 -m http.server 8080
# open http://localhost:8080
```

Serve it over HTTP rather than opening `index.html` straight from disk — a `file://` page can't fetch the live node data, so you'd only get the demo fallback.

## Data source

Live node data comes from [Node Scorecard](https://superpios.github.io/node-scorecard/), an open dashboard tracking speed, uptime, protocol and reliability across the Sentinel network.

## Learn more about Sentinel

- [sentinel.co](https://sentinel.co) — build your own dVPN
- [Run a node](https://docs.sentinel.co/dvpn-node-setup) and earn real $P2P as a node operator
- [x402.sentinel.co](https://x402.sentinel.co/) — dVPN for AI agents
- [P2PScan](https://p2pscan.com/) — every session and payment, on-chain and public

## Disclaimer

This is an unofficial, community-made project. It is not affiliated with, endorsed by, or sponsored by Sentinel P2P or by any of the applications it links to. All product names and links belong to their respective owners and are referenced here for educational purposes only. No third-party logos or brand assets are used — every graphic in the game is original.

No real cryptocurrency is distributed by this game. All in-game references to $P2P are purely educational and represent virtual points.

## Contributing

Found a factual error about the Sentinel ecosystem, or a broken link? Open an issue — accuracy matters more than polish here.

## License

MIT — see [LICENSE](LICENSE).
