# Aditya Joshi

**Founding engineer at two startups. I build the backends that keep real machines honest: freight trucks, EV fleets, and the full nodes that secure money.**

I get genuinely excited about the unglamorous layer: ingestion pipelines, deploy machinery, routing engines and protocol code. The stuff nobody notices until it breaks, and that I make sure doesn't. Go, Rust and TypeScript by day, cryptography and Solidity for fun.

<p>
<a href="https://www.linkedin.com/in/joshionchain/"><img src="https://img.shields.io/badge/LinkedIn-joshionchain-0A66C2?style=flat&logo=linkedin&logoColor=white" /></a>
<a href="https://x.com/JoshiOnChain"><img src="https://img.shields.io/badge/X-@JoshiOnChain-000000?style=flat&logo=x&logoColor=white" /></a>
<a href="https://ethresear.ch/u/codemongerrr/summary"><img src="https://img.shields.io/badge/ethresear.ch-codemongerrr-2b2b2b?style=flat&logo=ethereum&logoColor=white" /></a>
<a href="mailto:joshionchain@gmail.com"><img src="https://img.shields.io/badge/Email-joshionchain@gmail.com-EA4335?style=flat&logo=gmail&logoColor=white" /></a>
</p>

---

### Right now

#### BatteryFlow · Founding Engineer · Jun 2026 to present
EV fleet telemetry: a platform streaming millions of events a day from thousands of electric vehicles.

> Almost all of this lives in BatteryFlow's private GitLab, so the graph below barely sees it: **515 commits across ~20 repos in three months.** Here is what they bought.

- **All-India routing for about $30 a month.** Self-hosted OSRM doing 2,270 req/s on 2 vCPUs at a 4 ms median, instead of paying Google $5 per 1,000 requests.
- **A trip platform from zero.** Routes, corridor deviation, ETAs and alerts across 5 services, guarded by a 106,751-case differential test and a 2,297-case golden corpus that replays on every build.
- **A ghost in the telemetry.** Two devices on one vehicle were overwriting one Redis key. I built a rig that runs the deployed code verbatim, replayed 2.88M packets at 2,000-vehicle scale, counted 705k impossible-speed readings, and designed per-feed state lanes that took them to zero.
- **Production fixes on live ingestion**, including unblocking a partner feed that had rejected 613k packets.
- **BatteryFlow Rental, solo, in 18 days.** 181 commits: Cloudflare Workers and D1, HMAC-verified payment webhooks, and tenant-isolation tests that fail the build.

`TypeScript` `Deno` `Kafka` `Redis` `PostgreSQL` `MongoDB` `InfluxDB` `GraphQL` `OSRM` `GKE` `BigQuery` `Cloudflare Workers`

#### BharatTruck · Founding Engineer · Jan 2026 to present
A freight marketplace for Indian trucking, with a backend I built from the first commit.

- **7 services, a gateway and a unified app** on GCP Cloud Run and Supabase Postgres. I authored 125 of the first 126 merged PRs.
- **CI was green. Production wasn't.** Deploys had silently failed for 3 weeks after a monorepo move. I rebuilt the pipeline with post-deploy health probes, and it shipped 115 production deploys in the next 31 days.
- **A freight pricing engine in a day.** Four layers (cost floor, routed road distance, 60+ corridor market rates, quote reconciliation) that match the fleet's own cost model to 0.5% median error.
- **Pre-launch hardening:** closed 34 review findings in 2 weeks.

`TypeScript` `Fastify` `Next.js` `PostgreSQL` `Supabase` `Redis` `Cloud Run` `Cloud Build`

---

### Open source: Zcash

- **I wrote the two security fixes in [Zebra v6.2.2](https://github.com/ZcashFoundation/zebra/releases/tag/v6.2.2)**, the Zcash Foundation's full node. I took two open audit findings, reproduced a shell injection through the log filter with a crafted log line, rewrote the filter so log text never reaches a shell, and stopped a password leaking into the startup config dump. Both merged within 31 hours. ([#11050](https://github.com/ZcashFoundation/zebra/pull/11050), [#11051](https://github.com/ZcashFoundation/zebra/pull/11051))
- **4 merged PRs in Zebra**, and one of the 21 named contributors to [Zebra v6.4.0](https://zfnd.org/zebra-6-4-0-and-6-4-1-release/).
- Merged work in [librustzcash](https://github.com/zcash/librustzcash/pull/2624) and ZecHub, including a fix that brought 45 missing hackathon projects back to [zechub.wiki](https://github.com/ZecHub/zechub-wiki/pull/652).
- Dug into CI for Tachyon's [ragu](https://github.com/tachyon-zcash/ragu) and root-caused 16 straight failed fuzzing runs to a toolchain MSRV bump.

---

### Side quests

| Project | Stack | What it does |
|---|---|---|
| [**MEV-Shield**](https://github.com/CodeMongerrr/MEV-Shield) | TypeScript | Replays sandwich attacks in exact Uniswap V2 integer math on live mainnet reserves. Models why swaps under ~13 ETH are not worth attacking, then searches up to 1,100 public and private route splits per trade. |
| [**Weather-Telemetry**](https://github.com/CodeMongerrr/Weather-Telemetry) | TypeScript | Real-time telemetry pipeline: token-bucket rate-limited ingestion, Redis Streams consumers and a live feed. |
| [**CRC20-Token-Standards**](https://github.com/CodeMongerrr/CRC20-Token-Standards) | Solidity | Privacy-preserving token standard on Zama's fhEVM, built on fully homomorphic encryption. |
| [**Ring_Signature_Implementation**](https://github.com/CodeMongerrr/Ring_Signature_Implementation) | Rust | RSA ring signatures with a full sign and verify pipeline. |
| [**Load_Balancer**](https://github.com/CodeMongerrr/Load_Balancer) | Rust | Round-robin HTTP load balancer with health checks. |

---

### Before this

**Gusto Development** · Blockchain Developer Intern · Sep 2025 to Jan 2026

Janction DEX on JASMY Chain: AMM and DEX components, subgraph indexing on The Graph, and smart contract integrations.

**Nethermind** · Blockchain Engineer Intern · May to Aug 2024

[Juno](https://github.com/NethermindEth/juno), Nethermind's Starknet full node in Go, across the P2P, sync and RPC code paths.

---

### Tech I reach for

```
Languages   Go · Rust · TypeScript · Solidity · Python
Data        Kafka · Redis · PostgreSQL · MongoDB · InfluxDB · BigQuery · GraphQL
Infra       Docker · Kubernetes (GKE) · Cloud Run · Cloudflare Workers · CI/CD
Chain       Ethereum · Zcash · FHE (fhEVM) · ZK-SNARKs · MEV
```

IIT (ISM) Dhanbad · Mumbai

<p align="center"><img src="https://streak-stats.demolab.com/?user=CodeMongerrr&theme=transparent&hide_border=true" /></p>

<p align="center"><i>Working on hard backend, infra or protocol problems? I would love to hear about it.</i></p>
