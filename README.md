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



- **[Infoblox BloxOne Threat Defense](https://www.infoblox.com/)**  

  Enterprise protective DNS platform with threat intelligence feeds, DNS firewall, and Zero Day DNS detection. Blocks domains within 1-2 minutes of registration, eliminating the aging period for newly registered malicious domains . Available in Essentials, Business, and Advanced tiers with varying threat feed and protection levels . Features DNS tunneling/exfiltration blocking, DNS activity reporting, and cloud-based DNS firewall .



- **[Cisco Umbrella](https://umbrella.cisco.com/)**  

  Cloud-delivered security platform enforcing security at the DNS and IP layers, blocking malicious destinations before connection establishment . Trusted by 100+ million users, with 100% DNS service uptime and up to 73% latency reduction . Provides domain reputation scores, content filtering, and integrations with Cisco SIG. DNS Essentials starts at $1,960.08/license ; full Platform license at $284.99 .



- **[DNSFilter](https://www.dnsfilter.com/)**  

  Protective DNS and content filtering for enterprises, MSPs, and schools. Real-time threat detection spots threats 10 days faster than other feeds . Core plan starts at $1.00/license/month ($240/year minimum); Plus at $2.25/license/month ($750/year minimum) . Features DNS encryption (DNS-over-TLS), DNS PreCheck, CyberSight user behavior analytics, identity integrations (Entra ID/AD), and MCP Connector for AI assistant management .



- **[BlueCat](https://bluecatnetworks.com/)**  

  Unified DDI (DNS, DHCP, IPAM) platform with optional Threat Protection add-on enriching DNS data with crowdsourced intelligence . Features hub-and-spoke architecture managing thousands of DNS/DHCP servers from one appliance, 20-40% more LPS/QPS for equivalent resources, and role-based access controls . Trusted by government agencies for always-on operations and protection against DNS tunneling and DGA attacks .



- **[DNS Made Easy](https://dnsmadeeasy.com/)**  

  Enterprise DNS with proprietary Real-Time Traffic Anomaly Detection (RTTAD) using machine learning to identify unusual spikes, patterns, or DDoS events . Features flexible aggregation (global, regional, city/PoP level), custom alerts, and built-in DDoS protection at every PoP . Plans start at $50/month. Operates on AS16552 with true 100% uptime SLA and Tier 1 DDoS mitigation partnerships .



- **[NS1](https://ns1.com/)**  

  Intelligent DNS with DDoS resilience across 26 PoPs worldwide, backed by 100% uptime SLA . Features NS1 Trex™ nameserver software with near line-rate filtering for random Qname attacks, protocol filtering (drops non-DNS packets at edge), overbuilding/autoscaling to absorb attacks, and Super-POPs in key markets . DNSSEC signing without compromising traffic management .



- **[Cloudflare Gateway](https://www.cloudflare.com/zero-trust/products/gateway/)**  

  Zero Trust DNS filtering as part of Cloudflare One. Recommended deployment starts with DNS filtering (lowest effort, immediate protection): point network DNS to Gateway resolvers or deploy Cloudflare One Client in DNS-only mode; block security threat categories (malware, phishing, C2) and content categories violating acceptable use policy . Subsequent phases add network filtering, HTTP inspection with TLS decryption, and egress control .



- **[Control D](https://controld.com/)**  

  Cloud-based internet control panel offering granular DNS filtering beyond basic category blocking . Features device-specific profiles, service-level controls (block specific apps), custom rules (block/redirect/spoof specific domains, TLDs, or wildcards), scheduled behavior changes, and 100+ proxy exit locations . Positioned as a 30-second, zero-hardware alternative to Pi-hole . **Limitations**: Does not affect BitTorrent (P2P doesn't rely on DNS), cannot inspect page content (only domain lookups), and does not provide anonymity for life-critical use cases .



- **[WebTitan](https://www.titanhq.com/)**  

  DNS filtering and web security for businesses and MSPs. Effective web filtering blocking malicious and inappropriate sites, starting at $0.40/month . Used by organizations for 5+ years to resolve DNS issues with local providers .



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
