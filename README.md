# Awesome-DNS-Security

## Top DNS Security Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Protective DNS, Threat Intelligence & Encrypted DNS Filtering*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **DNS Security**. These tools block malicious domains, filter content, detect DNS tunneling and exfiltration, and provide visibility into DNS traffic for enterprises, MSPs, and educational institutions.



**Examples** include Infoblox, BloxOne Threat Defense, Cisco Umbrella, DNSFilter, BlueCat, DNS Made Easy, NS1, Cloudflare Gateway, Control D, and WebTitan (the category leaders).



**Open-source emphasis**: This section is expanded with active projects for self-hosting, custom blocklists, and transparent DNS filtering — ideal for privacy-conscious users, home labs, and organizations seeking vendor independence. The open-source ecosystem is anchored by **Pi-hole** (network-wide ad blocking), **AdGuard Home** (DNS filtering with parental controls), and **zdns** (privacy-focused DNS sinkhole), with strong coverage in encrypted DNS resolvers and DNS-over-TLS/HTTPS proxies.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Platform / Product | Company Size / Valuation | Starting Tier Pricing | Free Tier / Free Trial Limit | Key Features & Highlights |
| :--- | :--- | :--- | :--- | :--- |
| **[Cisco Umbrella](https://umbrella.cisco.com/)** | ~$425B Market Cap ($56.65B Revenue) | $1,960.08/year ($163.34/month for DNS Essentials 100-pack) or $5.00/user/month | 14-day free trial (up to 1,000 users/devices) | Cloud-delivered security platform enforcing policy at DNS & IP layers. Trusted by 100M+ users with 100% DNS service uptime, domain reputation scoring, and Cisco SIG integration. |
| **[NS1 (IBM NS1 Connect)](https://ns1.com/)** | ~$210B Market Cap ($62.0B Revenue) | $100.00/month (NS1 Essentials package) | 30-day free trial (full DNS routing & traffic steering functionality) | Intelligent DNS with DDoS resilience across 26 global PoPs, 100% uptime SLA, NS1 Trex™ near line-rate Qname attack filtering, and DNSSEC signing. |
| **[Cloudflare Gateway](https://www.cloudflare.com/zero-trust/products/gateway/)** | ~$125B Market Cap ($2.17B Revenue) | $0.00/month (Free Tier); Paid tiers start at $7.00/user/month | Free forever for up to 50 users (Cloudflare Zero Trust free plan) | Zero Trust DNS filtering part of Cloudflare One. Enforces security threat categories (malware, phishing, C2), acceptable use policies, and optional TLS decryption. |
| **[DNS Made Easy](https://dnsmadeeasy.com/)** | ~$8.0B Valuation ($500M Revenue) | $50.00/month (Business plan; entry tiers from $14.50/month) | 30-day free trial (full enterprise DNS management features) | Enterprise DNS with proprietary Real-Time Traffic Anomaly Detection (RTTAD) using ML to spot DDoS. Operates on AS16552 with true 100% uptime SLA. |
| **[Infoblox BloxOne Threat Defense](https://www.infoblox.com/)** | ~$3.4B Valuation ($1.0B ARR) | $1,500.00/year (~$125.00/month token-based starting baseline) | 30-day free trial (via cloud test drive & hands-on lab access) | Protective DNS with threat intelligence feeds, DNS firewall, and Zero-Day DNS detection. Blocks domains within 1–2 minutes of registration to stop aging malicious domains. |
| **[BlueCat](https://bluecatnetworks.com/)** | ~$1.8B Valuation (~$100M+ Revenue) | $500.00/month (Enterprise subscription baseline quote) | 30-day free trial (VM download for LiveAssurance / Horizon test drive) | Unified DDI (DNS, DHCP, IPAM) with optional Threat Protection add-on. Features hub-and-spoke architecture for enterprise DNS server management and DGA/tunneling protection. |
| **[WebTitan](https://www.titanhq.com/)** | ~$200M Valuation (~$30M Revenue) | $0.40/user/month ($240.00/year minimum contract) | 14-day free trial (full web & DNS filtering for unlimited test users) | DNS filtering and web security for businesses and MSPs. Effective category-based web filtering blocking malicious and inappropriate domains. |
| **[DNSFilter](https://www.dnsfilter.com/)** | ~$150M Valuation ($62M Funding, ~$40M Revenue) | $1.00/user/month ($240.00/year minimum contract for Basic plan) | 14-day free trial (no credit card required) | Protective DNS and content filtering for enterprises, MSPs, and schools. Real-time threat detection, DoT, PreCheck analytics, Entra ID integration, and MCP connector. |
| **[Control D](https://controld.com/)** | ~$20M Valuation (~$5M Revenue) | $2.00/endpoint/month (or $20.00/year personal plan) | 14-day free trial (full access to custom rules, profiles & proxy locations) | Cloud-based DNS control panel offering granular per-device profiles, app blocking, domain redirection/spoofing, scheduled policies, and 100+ proxy exit locations. |




## Open-Source GitHub Projects



- **[Pi-hole](https://github.com/pi-hole/pi-hole)**  

  The most widely adopted open-source network-wide ad and tracker blocking DNS sinkhole. Runs on Raspberry Pi or any Linux device, providing network-level filtering for all connected devices without client software. Features web-based admin interface, DHCP server integration, DNS-over-HTTPS support, and extensive community blocklists. **The de facto standard for self-hosted DNS filtering**.



- **[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)**  

  Open-source, network-wide DNS filtering solution with a modern web interface. Features DNS-over-TLS/HTTPS/QUIC support, parental controls, safe search enforcement, per-client configuration, and blocklists for ads, trackers, and malware. Cross-platform (Linux, macOS, Windows, Docker) with active development. **Strong alternative to Pi-hole with more granular per-client controls**.



- **[zdns](https://github.com/troubledcla/zdns)**  

  Privacy-focused DNS resolver and DNS sinkhole written in Go . Features DNS-level content filtering (similar to Pi-hole), parallel resolving over multiple resolvers, DNS-over-TLS/HTTPS for upstream protection, SQLite logging with REST API, Prometheus metrics, and zero run-time dependencies . Portable across VPS, container, laptop, Raspberry Pi, or home router . **Lightweight Go-based alternative for custom filtering workflows**.



- **[qdm12/dns](https://github.com/qdm12/dns)**  

  Docker-based DNS-over-TLS/HTTPS proxy and resolver with blocklist support . Features configurable blocklists for malicious IPs/hostnames, surveillance, and ads; custom block/allow lists for hostnames, IPs, and CIDRs; LRU caching; Prometheus metrics; and middleware for request/response logging . **Ideal for containerized environments needing encrypted DNS with filtering**.



- **[Blocky](https://github.com/0xERR0R/blocky)**  

  Fast and lightweight DNS proxy and ad-blocker for local networks. Features DoH/DoT support, blocklists, caching, per-client group configuration, Prometheus metrics, and DNS query logging. Written in Go with Docker deployment. **Modern alternative to Pi-hole with better performance characteristics**.



- **[Unbound](https://github.com/NLnetLabs/unbound)**  

  Validating, recursive, and caching DNS resolver with DNSSEC support. While not a filtering tool per se, it forms the foundation for many DNS security setups when combined with blocklist integrations. **The reference open-source DNS resolver**.



- **[Technitium DNS Server](https://github.com/TechnitiumSoftware/DnsServer)**  

  Self-hosted DNS server with web console, authoritative and recursive capabilities, block lists for ad/malware blocking, DoT/DoH/DoQ support, DNSSEC validation, and clustering. Serves 100,000+ requests per second on commodity hardware. **Full-featured self-hosted DNS server with built-in filtering**.



### Additional Strong Open-Source Options



- **DNSCrypt-proxy** — Flexible DNS proxy with support for DNSCrypt, DoH, and ODoH protocols, plus blocklist filtering and cloaking rules. Ideal for encrypted DNS on client devices.

- **dnsmasq** — Lightweight DNS forwarder and DHCP server with basic blocking via hosts files. Ubiquitous in router firmware but limited advanced filtering.

- **SmartDNS** — Local DNS server for bypassing geo-restrictions while providing basic ad blocking. Popular for streaming use cases.

- **NextDNS CLI** — Client for the NextDNS service (commercial with free tier) enabling encrypted DNS and filtering on routers and devices.



**Frameworks for building custom DNS security solutions**: Combine **Pi-hole** or **AdGuard Home** for network-wide filtering with web UI. Use **zdns** for a lightweight Go-based resolver with custom filtering logic and REST API. Deploy **qdm12/dns** in Docker environments needing encrypted DNS with blocklist support. Integrate **Blocky** for high-performance DNS proxying with per-client policies. Layer **Unbound** underneath for DNSSEC validation and recursion. Note that commercial platforms provide curated threat intelligence feeds, Zero Day DNS detection, and enterprise-grade DDoS resilience that open-source blocklists cannot replicate; open-source stacks excel at privacy-preserving filtering, custom blocklists, and self-hosted visibility.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- DNS security tools must comply with applicable laws regarding network monitoring, content filtering, and user privacy. Deploying filtering on networks without consent may violate regulations.

- Self-hosted open-source solutions require proper infrastructure, blocklist maintenance, and ongoing updates. DNS filtering at the domain level cannot inspect encrypted payloads or block content within allowed domains .

- The open-source ecosystem provides strong self-hosted filtering, encrypted DNS, and custom blocklist capabilities, but curated threat intelligence feeds, Zero Day DNS detection, and enterprise-grade DDoS resilience remain primarily commercial offerings.



---



**Made for network engineers, security analysts, privacy advocates, and self-hosting enthusiasts.**

Let's make DNS security more open, transparent, and user-controlled.
