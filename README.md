<p align="center">
<img alt="Aditya Joshi, forward deployed founding engineer" src="https://capsule-render.vercel.app/api?type=waving&height=190&color=0:0f172a,100:1e3a8a&text=Aditya%20Joshi&fontColor=e6edf3&fontSize=52&fontAlignY=36&desc=Forward%20deployed%20founding%20engineer&descAlignY=58&descSize=18" />
</p>

<p align="center">
<img alt="Hand me a messy business problem. I will find what is actually broken, then ship the system that fixes it." src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2600&pause=1400&color=58A6FF&center=true&vCenter=true&width=640&height=32&lines=Hand+me+a+messy+business+problem.;I+will+find+what+is+actually+broken,;then+ship+the+system+that+fixes+it." />
</p>

<p align="center">
<a href="https://www.linkedin.com/in/joshionchain/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-1e3a8a?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://x.com/JoshiOnChain"><img alt="X" src="https://img.shields.io/badge/X-1e3a8a?style=for-the-badge&logo=x&logoColor=white" /></a>
<a href="https://www.joshionchain.com"><img alt="Website" src="https://img.shields.io/badge/Website-1e3a8a?style=for-the-badge&logo=nextdotjs&logoColor=white" /></a>
<a href="mailto:joshionchain@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-1e3a8a?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

<p align="center">
<b>I own systems end to end, from first design to production.</b><br/>
Logistics · EV fleets · Crypto infrastructure<br/>
2 platforms built from scratch · ex-Nethermind · Zcash Zebra security fixes
</p>

---

### Now

#### BatteryFlow · Founding Engineer (Forward Deployed) · Jun 2026 to present
An EV fleet platform tracking **3,000+ electric vehicles** and **3.7M events a day**. I was brought in to find and fix its hardest problems.

> Almost all of this lives in BatteryFlow's private GitLab, so the contribution graph below barely sees it.

- **Route planning in 2 weeks.** A feature the team had never cracked, now powered by an in-house routing engine for all of India that handles **2,000+ routes a second on just 2 CPUs**, with 1,000x room to grow at a fixed cost.
- **Data operators can trust.** Revived a partner feed that had dropped **613k packets**, zeroed **705k impossible-speed readings** and ended **6.8M junk errors a week** sent to the partner, so alerts run on clean data.
- **Fleet onboarding.** Led onboarding for a national battery-swap network and a new OEM partner, then architected self-serve onboarding so business teams can launch new fleet customers without engineering in the loop.
- **A second product in 18 days.** Single-handedly built BatteryFlow Rental for riders and warehouses (181 commits, 38 PRs) with verified payment webhooks, OTP login and tenant-isolation tests that fail the build.

`TypeScript` `Kafka` `Redis` `PostgreSQL` `BigQuery` `Apollo GraphQL` `Kubernetes` `GCP`

---

### Previously

#### BharatTruck · Sole Founding Engineer · Jan to Aug 2026
An Indian freight marketplace for shippers, carriers and drivers. The founders brought the vision for scale, cost, legal and tax compliance. **I designed, built, hosted and ran every layer of it**, from zero to its first paid trip in production in 4 months.

- **Quotes that cover the real cost of a trip.** Replaced flat pricing that underpriced fuel by **38%** with a 4-layer pricing engine, built in one day, that matches the fleet's own cost model to **0.5% median error**.
- **Delivery restored.** Deploys had silently failed for 3 weeks. I rebuilt CI/CD with health probes, then shipped **115 production deploys in 31 days** across 7 microservices, authoring 125 of the first 126 PRs.
- **Accounts protected before launch.** Closed **34 review findings in 2 weeks** (11 PRs in a day), including open writes to the pricing tables behind every quote and reset tokens that worked as full logins.
- **Live truck tracking inside Google Maps' free tier.** One cached ETA call per trip every 45 seconds, so the mapping bill stays flat however many people watch a truck at once.

`TypeScript` `Fastify` `Next.js` `PostgreSQL` `Redis` `GCP` `CI/CD`

#### Gusto Development · Blockchain Developer (part-time) · Sep 2025 to Jan 2026
Custom-built swap execution for **Janction DEX**, a Uniswap V3-style exchange on JASMY Chain, around the client's Japan-specific market requirements that standard DEX logic could not handle, plus its Subgraph analytics.

#### Nethermind · Research Intern · May to Aug 2024
Joined the core-infrastructure team behind one of Ethereum's leading execution clients to work on [Juno](https://github.com/NethermindEth/juno), Nethermind's Go full node for Starknet, across P2P networking, chain sync and the JSON-RPC API. Chased a P2P bug where nodes never rejoined peers after going offline and briefed the core maintainers.

---

### Open source

- **Wrote both security fixes in [Zebra v6.2.2](https://github.com/ZcashFoundation/zebra/releases/tag/v6.2.2)**, the full node of a $26B+ privacy network, with both merged in 31 hours. One closed a shell-injection path so a malicious log line can no longer run commands on a node operator's machine ([#11050](https://github.com/ZcashFoundation/zebra/pull/11050)). The other stopped the Elasticsearch password leaking into the startup config dump ([#11051](https://github.com/ZcashFoundation/zebra/pull/11051)).
- **4 merged PRs in Zebra**, and one of the 21 named contributors to [Zebra v6.4.0](https://zfnd.org/zebra-6-4-0-and-6-4-1-release/).
- Merged work in [librustzcash](https://github.com/zcash/librustzcash/pull/2624) and ZecHub, including a fix that brought 45 missing hackathon projects back to [zechub.wiki](https://github.com/ZecHub/zechub-wiki/pull/652).

---

### Things I built on my own

- **[MEV Shield](https://github.com/CodeMongerrr/MEV-Shield)** · Cut the modeled sandwich-attack loss on a **$660K (250 ETH) swap** from $35.9K to under $1K, a **97% reduction**, by simulating the attacking bot on live Ethereum data and picking the cheapest safe route. [Live demo](https://mev-shield.joshionchain.workers.dev)
- **[Earshot](https://www.npmjs.com/package/@jino-labs/earshot)** · Watch and steer Claude Code agent sessions across machines from one page, **end-to-end encrypted** so the relay never sees code or prompts, with guest links that can watch but never issue commands. Published on npm with zero runtime dependencies.
- **[Streaming ingest pipeline](https://github.com/CodeMongerrr/stream-ingest-pipeline)** · Crash-safe ingestion with Redis Streams consumer groups, 50 async workers and one atomic rate limiter shared across every replica, so scaling out never breaks the upstream quota.
- **[GKE on Terraform](https://github.com/CodeMongerrr/GKE-Kubernetes)** · Infrastructure as code for Google Kubernetes Engine, with Kustomize overlays, smoke tests that roll back automatically, disruption budgets and anti-affinity.

---

### Skills

<p align="center">
<img alt="Tech stack" src="https://skillicons.dev/icons?i=ts,py,go,rust,solidity,nodejs,react,nextjs,graphql,kafka,redis,postgres,kubernetes,gcp,terraform&perline=15" />
</p>

- **Languages and frameworks** · TypeScript, Python, Go, Rust, SQL, Solidity, Node.js, Fastify, React, Next.js, Apollo GraphQL
- **AI engineering** · LLM agents, tool calling, RAG, vector search, MCP servers, Claude Agent SDK, structured outputs, guardrails
- **Distributed systems** · Event-driven microservices, Kafka, Redis, PostgreSQL, BigQuery, Kubernetes, GCP, Terraform, CI/CD
- **Web3 and security** · Ethereum, smart contracts, DeFi, MEV, Zcash, Starknet, P2P networking, application security, tenant isolation

IIT (ISM) Dhanbad · Integrated Master of Technology · class of 2026 · Mumbai, open to relocation (US, UK, UAE)

<p align="center"><i>Got a problem where the hard part is figuring out what is actually broken? I would love to hear about it.</i></p>
