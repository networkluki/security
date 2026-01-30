# security

**Server Hardening & Cloudflare Architecture**

Technical documentation for securing Linux servers using a layered,
defense-in-depth approach with Cloudflare as an edge security provider.

This repository focuses on practical, reproducible security practices
rather than theory or vendor-specific marketing.

---

## Overview

This project documents a hardened server architecture designed for
internet-exposed Linux systems. The goal is to reduce attack surface,
limit blast radius, and improve observability in hostile environments.

Core focus areas:

- Operating system hardening
- Network-level protection
- Secure service configuration
- Cloudflare edge security integration
- Logging and monitoring

---

## Scope & Threat Model

### Assumptions

- Public-facing Linux servers
- Continuous background scanning and probing
- Untrusted client networks
- Automated attack traffic is expected

### In Scope

- SSH brute-force mitigation
- Service exposure reduction
- Firewall and network filtering
- Web server hardening
- Cloudflare-based edge protection

### Out of Scope

- Zero-day exploitation
- Physical access attacks
- Insider threats
- Nation-state level adversaries

---

## Architecture

High-level security layers:

1. Cloudflare (DNS, WAF, rate limiting, TLS termination)
2. Network firewall (iptables / nftables)
3. Operating system hardening
4. Application-layer security (Apache / PHP)
5. Logging, monitoring, and alerting

