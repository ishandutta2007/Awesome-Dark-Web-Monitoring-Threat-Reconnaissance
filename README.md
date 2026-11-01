# Awesome-Dark-Web-Monitoring-Threat-Reconnaissance

# Awesome-Dark-Web-Monitoring-Threat-Reconnaissance

**Top Dark Web Monitoring Threat Reconnaissance (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Illicit Community Collection, Credential Exposure, Threat Actor Tracking & Self-Hosted Dark Web OSINT*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Dark Web Monitoring & Threat Reconnaissance**. These tools enable security teams to monitor criminal forums, paste sites, and Tor-hidden services for leaked credentials, brand abuse, and threat actor chatter—from fully managed enterprise platforms with proprietary dark web collection to self-hosted OSINT tools that give researchers control over their reconnaissance pipeline.



**Examples** include CrowdStrike Falcon Intelligence Recon, Recorded Future, Flashpoint, ZeroFox, Cybersixgill, SpyCloud, Flare Systems, DarkOwl, SOCRadar, and KELA (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted dark web reconnaissance, credential monitoring, and open OSINT infrastructure. **Critical note**: The open-source landscape is sparse—**voidaccess** is the only purpose-built self-hosted dark web OSINT platform, but it is a newer project with limited production validation . **IVRE** provides network reconnaissance (not dark web), and **MISP** handles intelligence sharing rather than collection. No open-source project matches Recorded Future's Intelligence Graph or Flashpoint's illicit community access.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CrowdStrike Falcon Intelligence Recon](https://www.crowdstrike.com/)**

  **Dark web and brand monitoring** within Falcon Intelligence. **Pricing**: **Custom quote only**—no public pricing, no free tier . Support tier premiums add ~$10,000/year, capped at 12% of license cost . **Free tier**: None. **Best for**: CrowdStrike customers wanting recon integrated with Falcon telemetry—**trade-off**: quote-only; requires existing Falcon investment.



- **[Recorded Future](https://www.recordedfuture.com/)**

  **Intelligence platform** with dark web and technical collection. **Pricing**: **Quote-only**; UK G-Cloud listing shows **no discount tiers up to £5M+** and a **30-day sandbox trial on request** . **Free tier**: Trial sandbox only. **Best for**: enterprises wanting comprehensive intelligence including dark web—**trade-off**: no self-serve; procurement requires sales engagement.



- **[Flashpoint](https://flashpoint.io/)**

  **Threat intelligence platform** with illicit community collection. **Pricing**: **Quote-only**; Vendr median buyer pays **$57,855/year** (range $54,200–$79,730) . Core packages include **Cyber Threat Intelligence** (Ignite, API, account takeover credentials, vulnerability intelligence) and **Physical Security** (Echosec) . Claims **482% ROI in 6 months** and **$500M fraud loss avoided per year** . **Free tier**: None. **Best for**: CTI and fraud teams needing broad illicit-source coverage—**trade-off**: enterprise pricing; value depends on dark web relevance.



- **[ZeroFox](https://www.zerofox.com/)**

  **Digital risk protection** with dark web monitoring and takedown capability. **Pricing**: **Quote-only**; outcome-based, not per-headcount. **Free tier**: None. **Best for**: organizations prioritizing brand protection and takedowns alongside intelligence—**trade-off**: digital risk focus; less depth in pure adversary tracking.



- **[Cybersixgill](https://cybersixgill.com/)**

  **Dark web intelligence** platform with Investigative Portal. **Pricing**: **Quote-only**; TrustRadius shows **no free trial and no freemium version** . **Free tier**: None. **Best for**: teams needing deep dark web coverage—**trade-off**: no trial; portal-centric.



- **[SpyCloud](https://spycloud.com/)**

  **Account takeover prevention** with credential exposure monitoring. **Pricing**: **Custom quote, negotiable**; **no published pricing, no self-serve checkout, no free tier** . SMB tier (1–99 mailboxes) buried in **reseller pricelists**, not advertised . **Free tier**: **No**—free exposure scan tool only. **Best for**: enterprises fighting account takeover—**trade-off**: sales-led, no transparent pricing; skip if you want self-serve.



- **[Flare Systems](https://flare.io/)**

  **Threat exposure management** monitoring clear and dark web, Telegram, and cybercrime forums for leaked credentials and stealer logs. **Pricing**: **Quote-based**; **free trial available** . Scores **82.8/100 in 2026 Infostealer Index**—leading on specialization, machine context, segmentation, and sessions . **Free tier**: Trial available. **Best for**: security teams wanting fast-to-deploy exposure monitoring with stealer-log context—**trade-off**: quote-based; smaller vendor than Recorded Future.



- **[DarkOwl](https://www.darkowl.com/)**

  **Dark web intelligence** with Vision UI, Search API, Entity API, Score API, and Datafeeds. **Pricing**: **All 5 plans quote-only**; buyers report **starting from ~$38,000/year** (4 public sources) . **No free plan, no trial**; **auto-renew with 12/24/36-month minimums**; **3–5% or 5–10% annual price escalation**; 30/60/90-day cancellation notice . **Free tier**: None. **Best for**: teams wanting dark web data via API or UI—**trade-off**: no trial; auto-renewal with escalation; 7 documented hidden costs .



- **[SOCRadar](https://socradar.io/)**

  **Cyber threat intelligence** with dark web monitoring. **Pricing**: **Essential $14,750/year** (vulnerability intel, dark web intel, threat hunting, 1,000 search credits, 1 supply chain vendor, 50+ feeds, 6,000+ combolists, 100 malware analysis credits); **Freemium $0** available . **Free tier**: Yes, Freemium plan. **Best for**: SMBs wanting affordable CTI with dark web monitoring—**trade-off**: Essential credits limited; Freemium scope unverified.



- **[KELA](https://www.kela.io/)**

  **Dark web threat intelligence** platform. **Pricing**: Quote-only. **Free tier**: None. **Best for**: enterprises wanting curated dark web intelligence—**trade-off**: no public pricing; sales-led.



## Open-Source GitHub Projects



- **[voidaccess](https://github.com/KatrielMoses/voidaccess)**

  **Self-hosted dark web OSINT platform** (license per repo) — **the only purpose-built open-source dark web reconnaissance tool** found in this research, positioned as a free alternative to Recorded Future, DarkOwl, and Flare . **Features**: **One query fans out to 12+ Tor search engines**, code hosts, security feeds, and curated `.onion` seeds; **follows new .onion links** as it finds them; **mandatory safety gates** drop prohibited queries, URLs, and content; **extracts entities** (threat actors, infrastructure, crypto wallets, credentials masked, messaging handles, CVEs); **links entities into a searchable relationship graph** with communities and infrastructure clusters; **exports** to STIX, MISP, Sigma, YARA, Snort, Suricata, CSV, Markdown, JSON; **CLI** (`voidaccess investigate`, `export`, `show`, `enrich`); **hosted version** at voidaccess.pro . **Tech stack**: Python 3.10+, PostgreSQL, Tor, Docker Compose for full stack . **Deploy**: `pip install voidaccess` or Docker Compose self-hosting . **Trade-off**: **Newer project**—limited production validation; hosted version routes through Tor on vendor servers; clearnet-only mode available without Tor. **Best for**: security researchers and threat-intel teams wanting a free, self-hosted dark web OSINT pipeline with graph output and STIX/MISP export—especially those priced out of Recorded Future or DarkOwl.



### Additional Strong Open-Source Options



- **IVRE** — Network recon framework (GPL-3.0, ~4,068 stars). Build self-hosted alternatives to Shodan/Censys with Nmap, Masscan, Zeek, and Passive DNS. **Note**: **Network reconnaissance, not dark web**—internet-wide scanning, not Tor/illicit forums . **Best for**: teams building their own internet scanning infrastructure.

- **MISP** — Threat intelligence sharing platform (AGPL-3.0). IOC management, correlation, sharing communities. **Note**: **Sharing and intelligence management, not dark web collection**—pair with voidaccess for collection. **Best for**: ISACs and teams needing intelligence sharing infrastructure.

- **No mature open-source dark web monitoring platform exists beyond voidaccess.** The category is dominated by proprietary vendors with proprietary collection networks and analyst teams. **voidaccess** provides a functional starting point but lacks the source breadth and validation of commercial platforms.



**Frameworks for building custom systems**: **voidaccess** is the only open-source dark web OSINT tool. Pair it with **MISP** for intelligence sharing and **IVRE** for clearnet reconnaissance—creating a limited open-source recon stack. **None of these match Flashpoint's illicit community access or Recorded Future's Intelligence Graph.**



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Dark web monitoring platforms handle sensitive intelligence and credential data. Accessing dark web forums may have legal implications depending on jurisdiction. **Ensure your use complies with applicable laws and your organization's authorized investigation policies.**

- **The "illicit community collection" vs. "credential exposure" vs. "digital risk protection" vs. "self-hosted OSINT" distinction is critical.** **Flashpoint and KELA** are **illicit community collection**—they provide access to criminal forums and markets . **SpyCloud** is **credential exposure**—it focuses on account takeover and leaked credentials . **ZeroFox** is **digital risk protection**—brand protection and takedowns . **voidaccess** is **self-hosted OSINT**—it collects from Tor and open sources but lacks proprietary forum access . **Choose based on whether you need forum access, credential monitoring, brand protection, or self-hosted recon.**

- **SpyCloud has no free tier and no self-serve checkout.** SMB pricing is buried in reseller pricelists—**skip if you want transparent pricing** . **Flare offers a free trial with fast time-to-value** .

- **DarkOwl auto-renews with 12/24/36-month minimums and 3–10% annual escalation.** Buyers report **~$38K/year starting**, but hidden costs (implementation, training, add-ons) add significantly . **Negotiate escalation caps and cancellation terms before signing.**

- **Flashpoint's median buyer pays $57,855/year** (range $54,200–$79,730) . Claims **482% ROI** and **$500M fraud avoided** are vendor-reported—validate against your own threat model .

- **SOCRadar Essential at $14,750/year is the most transparent entry point** in this category, with a **Freemium $0** option . **For SMBs testing dark web monitoring, it is the pragmatic starting point.**

- **voidaccess is the only open-source dark web OSINT tool**, but it is **newer with limited validation** . The hosted version routes through Tor on vendor servers; self-hosting requires PostgreSQL and Docker Compose . **For researchers wanting a free alternative to commercial platforms, it is the starting point.**

- **Pricing opacity is universal** across CrowdStrike, Recorded Future, Flashpoint, ZeroFox, Cybersixgill, SpyCloud, Flare, DarkOwl, and KELA. All require sales contact or quote requests. **SOCRadar publishes Essential pricing.** **Validate with direct vendor conversations against your threat model and collection requirements.**

- Self-hosted open-source solutions require proper infrastructure (PostgreSQL, Tor for voidaccess), security hardening, and ongoing maintenance. **Dark web reconnaissance involves interacting with criminal infrastructure**—ensure your deployment is isolated and meets your organization's legal and security standards before collecting intelligence.



---



**Made for threat intelligence analysts, security researchers, and organizations building transparent dark web reconnaissance solutions.**

Let's make Dark Web Monitoring & Threat Reconnaissance more open, data-driven, and adversary-aware.
