# Sentinel Node Dash

An arcade endless-runner that teaches the **Sentinel dVPN ecosystem** while you play — powered by **live node data**.

**▶ Play: https://superpios.github.io/sentinel-node-dash/**

---

## What it is

You are a data packet running through the Sentinel decentralized bandwidth network.

- ⚡ **Collect real nodes.** Every node orb is a live Sentinel node pulled from the [Node Scorecard](https://superpios.github.io/node-scorecard/) — real moniker, real country, real download speed, real protocol (WireGuard / V2Ray).
- ⭐ **Residential nodes pay x2.4.** Nodes on real home connections (`hosting: false`) are the top privacy tier — their IP looks like a normal user, so they're far harder to block. Datacenter nodes pay x1.2: huge bandwidth, but known IP ranges.
- ⚠️ **Dodge the censorship bricks.** DPI, trackers, ISP logs, geo-blocks, throttling.
- 🎮 Three player skins, pause / restart / main menu from anywhere, double jump, synthesized chiptune audio.
- ⭐ **Unlock the ecosystem — 22 topics.** Stars reveal the dVPN apps built on Sentinel (Sentinel Shield, Independent VPN, Ryn VPN, DVPN by NORSE, VALT, Meile, ChibaTunnel), the tools and explorers (BlueCLI, P2PScan, SuchNode, Network Stats, Node Scorecard), the community (Bluefrens), and the concepts that make it all work: on-chain sessions, $P2P, WireGuard/V2Ray, the incoming anti-censorship protocols, and x402 payments for AI agents.
  Each topic — and its quiz — appears **only once per run**. Once you've seen them all, stars become pure bonus and the game never interrupts you again.

## Tech

- **Single HTML file.** No build step, no framework, no CDN, no dependencies.
- **No tracking, no analytics, no cookies.** Only one outbound request: the public Node Scorecard JSON.
- Audio is synthesized in-browser with the Web Audio API — no media files.
- All artwork is original vector art drawn on `<canvas>`. No third-party logos or trademark files are embedded.
- Falls back to demo node data if the Scorecard is unreachable, so the game always runs.

## Run locally

```bash
git clone https://github.com/superpios/sentinel-node-dash.git
cd sentinel-node-dash
python3 -m http.server 8080
# open http://localhost:8080
```

## Data source

Live node data: [`node-scorecard/latest.json`](https://superpios.github.io/node-scorecard/) — an open dashboard tracking speed, uptime, protocol and reliability across the Sentinel network.

## Learn more

- [sentinel.co](https://sentinel.co) — build your own dVPN
- [Run a node](https://docs.sentinel.co/dvpn-node-setup) and earn $P2P
- [x402.sentinel.co](https://x402.sentinel.co/) — dVPN for AI agents

## License

MIT — see [LICENSE](LICENSE).
